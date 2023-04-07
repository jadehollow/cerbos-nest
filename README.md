# Cerbos NestJS Demo

This demo project uses Cerbos in NestJS as an interceptor to validate requests based on policies defined in Cerbos.

Note! You should NOT use authentication as demonstrated, a JWT Guard in NestJS is recommended.

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod

# cerbos
$ npm run cerbos:start

# cerbos & dev
$ npm run start:devcerbos
```

## Requests

As admin:
`curl -H "Authorization: admin" http://localhost:3000/document/1`

As user:
`curl -H "Authorization: user" http://localhost:3000/document/1`

You can change between documents 1-3 to test different policies as different users.

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```
