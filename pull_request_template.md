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
- Test the changes
- After testing, run `npx prisma migrate dev --name [name-here]` to generate a migration
- Run `npx prisma generate`
- Commit and push up changes

_Collaborators: If the Prisma schema changed, pull down the changes locally. Then, run `npx prisma migrate dev` to update your local testing database - [Prisma Docs](https://www.prisma.io/docs/orm/prisma-migrate/workflows/team-development)_

#### New Project
**If the migrations folder does not yet exist, follow these steps:**
- Run `npx prisma migrate dev`
  - name: init
- Run `npx prisma generate`
- The project is now ready to follow the Schema Change Workflow, as needed

### Before

<!-- If UI feature, please provide 'before' screenshots -->

### After

<!-- If UI feature, please provide 'after' screenshots -->

#### Share a GIF

<!--- Add a GIF --->

![Coding Rocks](https://media.giphy.com/media/24652QfeZzNIPzoH36/giphy.gif)
