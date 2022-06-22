### Development guide

- Start up PostgreSQL server somewhere (use https://hub.docker.com/_/postgres/)
- Install dependencies (`npm i`)
- Create `.env` containing `DATABASE_URL` similar to `.env copy`, append `/mydb?schema=public` to target `mydb` database's `public` schema.
- Run `npx prisma db push` to push schema to database, and run `npx prisma generate` if it doesn't do that already to create Prisma Client
- `npm run dev` to start up dev server!
