# [Project Name]

<!-- <img src="./public/logo.svg" alt="Logo" width="350px"> -->

## Table of Contents

|     |                                             |
| --- | ------------------------------------------- |
| 1.  | [Description](#description)                 |
| 2.  | [LCNW Staff Involved](#lcnw-staff-involved) |
| 3.  | [Wiki And Resources](#wiki-and-resources)   |
| 4.  | [Functionality](#functionality)             |
| 5.  | [Branches](#branches)                       |
| 6.  | [Database Set Up](#database-set-up)         |
| 7.  | [Development Set Up](#development-set-up)   |
| 8.  | [Tools](#tools)                             |
| 9.  | [Deployment](#deployment)                   |

## Description:

Created: [date]

Deployed: [date]

[description]

## LCNW Staff Involved

- Developers: [names]
- Stakeholder: [names]

## Wiki And Resources

- [Project Name Wiki]()

## Functionality:

- [List functionality]

## Branches

| Branch Name | Deployment Links | Action  |
| ----------- | ---------------- | ------- |
| main        | [Production]()   | on push |
| development | [Development]()  | on push |

## Database Set Up

1. Create a testing database in pgAdmin
2. In root directory run `npx prisma db push` to create tables in pgAdmin

## Database Schema

[brief schema description]

<!-- <img src="./public/schema.png" alt="DB Schema" width="450px"> -->

_To generate a schema image like the one above: In pgAdmin, right click the
desired database. Then, select 'Generate ERD' and 'Download Image'_

## Development Set Up

1. Clone branch
2. `npm install`
3. Create .env file in root directory and add env variables:

```
NEXT_PUBLIC_DEV=true
NEXT_PUBLIC_PROD=false
DATABASE_URL="postgresql://[username]:[password]@localhost:5432/teamtest?schema=public"
```

Please check in 1pass or reach out to a fellow developer for env variable
values.

4. Fire up localhost:3000: `npm run dev`
5. Create new branch off of main: `git checkout -b branch-name`

## Local Development Notes

[notes, if needed]

## Tools

- [Next.js: framework](https://nextjs.org/docs/getting-started)
- [NextAuth.js](https://next-auth.js.org/)
- [Prisma: ORM](https://www.prisma.io/)
- [Tailwind CSS](https://tailwindcss.com/)
- [additional tools here]

## Deployment

Deployed using Azure App Services on Linux containers and Azure Postgres
flexible servers.

## CI/CD Workflow

Using GitHub Actions:

- Pushing or merging branches to the **_development branch_** will trigger the CI/CD
  pipeline to build and deploy to the development azure container.
- Pushing or merging branches to the **_main branch_** will trigger the CI/CD
  pipeline to build and deploy to the production azure container.
- Pushing or merging to either of those branches also runs the command
  `npx prisma migrate deploy` which keeps all databases in sync with the Prisma
  Schema.
- Pushing to either of those branches with only changes to .md files will not
  trigger deployment cycles.
