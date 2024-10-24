# Overview

- Built off [T3 Stack](https://create.t3.gg/): TypeScript, Tailwind CS v3, Next.js v14, NextAuth.js, Prisma ORM, Postgres, tRPC
- Shadcn UI
- `.cursorrules` setup
- eslint and prettier, husky precommit linter,
- local postgres database
- local temporal server
- Typescript script runner with env variables(run-script)
- declarative routing with zod, @/utils/router/routes

## Running the app

1. Start up development database
2. Run Prisma Migrate, if needed
3. Start the app

```
pnpm run dev:services:up #1
pnpm prisma migrate dev #2
pnpm run dev #3
```

Go to http://localhost:3000/ to see the app.

## Setup

Rename `sample.env` to `.env`

### Other commands

Run this command to cleanup the codebase or your commit will be rejected:

```
pnpm run format
pnpm prisma studio
```

Go to http://localhost:8233 to see temporal web ui.

## Setup

- Install pnpm and have Docker running

```
pnpm install
```

### Environment Variables

Add to env.js.
