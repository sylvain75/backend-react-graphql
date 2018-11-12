# backend-react-graphql

- Follow the steps: https://www.prisma.io/docs/quickstart/
- Create a `variables.env` + the following keys: (it will be used in `prisma.graphql`)
  - PRISMA_ENDPOINT="urlgeneratedbyprisma"
  - PRISMA_SECRET="something"
- After deploying `prisma deploy --env-file variables.env` copy/paste the url given for the prisma graphql playground

### Running Yoga
prisma server: `db.js` has typeDefs plugged to the generated `prisma.graphql` file => reason why there is a hook creating it
yoga server: `createServer.js` has differents typeDefs => confusing

run `npm run debug`