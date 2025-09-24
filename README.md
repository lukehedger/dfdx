# dfdx

durable functions dx

## Prerequisites

- Install [Bun](https://bun.sh/)
- Publish [Bun runtime Lambda layer](https://github.com/oven-sh/bun/blob/main/packages/bun-lambda/README.md#setup)

## Develop

To start a local Bun server, run `bun index.ts`.

Or, to enable hot reloading run `bun index.ts --hot`.

### Test

To test the function locally, run `curl -X POST -H "Content-Type: application/json" -d '{"test": true}' http://localhost:3000`.

## Deploy

Run `bunx cdk deploy` to deploy the CDK stack to your AWS account.

### Test

To test the deployed function, run `curl -X POST -H "Content-Type: application/json" -d '{"test": true}' <API_GATEWAY_URL>`.
