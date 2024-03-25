### Description

<!-- What does this code change? Anything else to share? -->

### Merge Time

<!-- Can this be merged immediately or does it need to wait? -->

### Review

<!-- Pair review or solo review? -->

### Schema Change

<!-- Did the schema change? If not, remove this entire section -->

#### Schema Change Workflow
- Make desired changes to the `schema.prisma` file
- Run the command `npx prisma db push` to update the database locally
- Test the changes
- After testing, run `npx prisma migrate dev --name [name-here]` to generate a migration
- Commit and push up changes

_Collaborators: If the Prisma schema changed, pull down the changes locally. Then, run `npx prisma migrate dev` to update your local testing database - [Prisma Docs](https://www.prisma.io/docs/orm/prisma-migrate/workflows/team-development)_

### Before

<!-- If UI feature, please provide 'before' screenshots -->

### After

<!-- If UI feature, please provide 'after' screenshots -->

#### Share a GIF

<!--- Add a GIF --->

![Coding Rocks](https://media.giphy.com/media/24652QfeZzNIPzoH36/giphy.gif)
