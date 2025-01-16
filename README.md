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
```
