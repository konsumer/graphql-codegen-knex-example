# graphql-codegen-knex-example

# WORK IN PROGRESS

This project illustrates the use of [graphql-codegen-knex-migration](https://github.com/konsumer/graphql-codegen-knex-migration) to create knex migrations and [graphql-codegen-knex-joinmonster](https://github.com/konsumer/graphql-codegen-knex-joinmonster) to create the join-monster meta info that matches this.

## usage

```
git clone https://github.com/konsumer/graphql-codegen-knex-example.git
cd graphql-codegen-knex-example
npm i            # install dev-dependencies
npm run generate # run graphql-codegen to generate migrations & join-monster info
npm start        # start the example server
```


To use this setup in your project:

```
npm i -D knex @graphql-codegen/cli graphql graphql-codegen-knex-joinmonster graphql-codegen-knex-migration
npm i graphql-type-json graphql-iso-date
```

* Copy `schema/_codegen.graphql` into your project
* Copy the directives from `resolvers/schemaDirectives.js` into your project
* Have a look at `server.js` for ideas on how to setup your GraphQL server
* Have a look at `codegen.yml` for ideas on how to use the plugins
* Have a look at `package.json` `scripts` for action-recipes.