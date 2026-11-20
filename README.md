# odin-prisma-practice
Odin Project, NodeJS Course, ORMs, Prisma ORM

Main schema is in `./prisma/schema.prisma`<br>
Connector/adapter (from this local project's prisma to DB) is in `./lib/prisma.js`<br>
Prisma code (to add entries/query the DB) is in `./script.js`<br>

Note: if you want to see the tables synced over to the PostGreSQL DB, you need to prefix the table name with `public.` and use quotes around the table name. For example: `select * from public."Post";`


installed packages:<br>
`npm install prisma@prev --save-dev`<br>
`npm install @prisma/client@7 @prisma/adapter-pg pg dotenv`<br>

`npx prisma` to view some handy commands + check if installed correctly (optional)<br>

`npx prisma migrate dev --name init` to migrate/sync schema tables over to DB (`--name init` just names the migration "init", and is not needed after the first migration)<br>
`npx prisma generate` to generate Prisma files (for the schema tables?)<br>

`node script.js` to run script.js, adding a new user to the DB table and printing all users to terminal<br>
`npx prisma studio` opens a browser visual of DB table<br>
