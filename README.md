# Blood Donor & Emergency Request Network

A platform connecting blood donors with people posting urgent blood requests,
matched by blood group and location.

## Stack

- **Framework:** Next.js (App Router, JavaScript) — frontend and backend API
  routes live in one project
- **Database:** MySQL
- **ORM:** Prisma

## Getting Started (local development)

1. Install dependencies:
   ```bash
   npm install
   ```
2. Copy `.env.example` to `.env` and fill in your MySQL connection string:
   ```bash
   cp .env.example .env
   ```
3. Run the dev server:
   ```bash
   npm run dev
   ```
4. Open [http://localhost:3000](http://localhost:3000).

## Database

The Prisma schema lives in `prisma/schema.prisma`. Once models are added:

```bash
npx prisma migrate dev --name <change-name>   # create/apply a migration
npx prisma generate                           # regenerate the Prisma client
npx prisma studio                              # browse the database in a UI
```

`.env` is not committed (see `.env.example` for the expected variable).
