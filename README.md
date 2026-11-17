# odin-prisma-practice
Odin Project, NodeJS Course, ORMs, Prisma ORM

Main schema is in `./prisma/schema.prisma`
Connector/adapter (from this local project's prisma to DB) is in `./lib/prisma.js`
Prisma code (to add entries/query the DB) is in `./script.js`

Note: using the installation instructions below, don't create a `.env` file, it creates one automatically during `npx prisma init ...`


installed packages:
`npm install prisma@prev --save-dev`
`npm install @prisma/client@7 @prisma/adapter-pg pg dotenv`

`npx prisma` to view some handy commands + check if installed correctly (optional)

`npx prisma migrate dev --name init` to create (compile?) schema tables
`npx prisma generate` to generate Prisma files (for the schema tables?)

`node script.js` to run script.js, adding a new user to the DB table and printing all users to terminal
`npx prisma studio` opens a browser visual of DB table
