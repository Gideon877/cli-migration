# cli-migration


##### Creating environment variables file

> Create a .env file in the root directory of your project. Add environment-specific variables on new lines in the form of NAME=VALUE. For example:

```bash
DB_HOST=localhost
DATABASE_URL=postgresql://localhost:${PORT}/${DATABASE_NAME}
```

##### Install package as dev dependency

> npm install --save-dev postgres-migration

##### Usage 

> ### `structure`

```bash
.
+-- node_modules
+-- src
|   +-- *.js
+-- sql
|   +-- 001-create-user-table.sql
|   +-- 002-alter-user-table.sql
+-- index.html
+-- package.json
```

###### In terminal

```bash
postgres-migration
```

or 

```json
{
  "script": {
      "migrate": "postgres-migration"
  }
}
```

###### run following command to excute

> npm run migrate

