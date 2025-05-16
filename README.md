
# Provider 

because the pact contract testing is only free for the first 30 days now, this is the continuation of the course but without he contract testing disabled.

[![API Documentation](https://img.shields.io/badge/API-DOCUMENTATION-blue?style=flat-square)](https://muratkeremozcan.github.io/provider/api-docs.html)

## Setup

```bash
npm i
```

Use the sample `.env.example` file to create a `.env` file of your own. These values will also have to exist in your CI secrets.

```bash
PORT=3001
```

### Scripts

```bash
npm run lint
npm run typecheck
npm run fix:format
npm run validate # all the above in parallel

npm run test # unit tests
npm run test:watch # watch mode

npm run mock:server # starts the mock backend/provider server

npm run cy:open-local # open mode
npm run cy:run-local  # run mode
npm run cy:run-local-fast  # no video or screen shots
```
# provider-pw-start

npm init playwright@latest

1. playwright related commands
```bash
    "pw:open": "npx playwright test --ui",
    "pw:open-local": "npx playwright test --ui -c pw/config/local.config.ts",
    "pw:open-local-debug": "PWDEBUG=1 npx playwright test --ui -c pw/config/local.config.ts",
    "pw:run-local": "npx playwright test -c pw/config/local.config.ts",
    "pw:run-local-trace": "npx playwright test --trace on && npx playwright show-report -c pw/config/local.config.ts",
    "pw:open-local-trace": "npx playwright show-trace -c pw/config/local.config.ts"
```
