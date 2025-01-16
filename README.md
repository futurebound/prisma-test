# Prisma Test

Testing repo for Prisma ORM.

## Setup

```shell
pnpm add -D prisma typescript ts-node @types/node

#
pnpm dlx prisma init --datasource-provider postgresql

# Map data model to database schema
# 1) Creates new SQL migration file
# 2) Runs SQL migration file against database
pnpm dlx prisma migrate dev --name init

#
pnpm add @prisma/client
```

![](https://www.prisma.io/docs/assets/images/prisma-client-install-and-generate-ece3e0733edc615e416d6d654c05e980.png)

## Updating Schema

Whenever you update Prisma schema, must update database schema with either:

- `prisma migrate dev`
- `prisma db push`

Keeps database schema in sync with Prisma schema, and regenerates Prisma Client.
