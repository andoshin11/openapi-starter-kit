# Open API Starter Kit
This template comes with

- [swagpack](https://www.npmjs.com/package/swagpack)
- [Swagger UI](https://swagger.io/tools/swagger-ui/)
- linting setup

## Setup
TBD

## Testing
TBD

## Linting
TBD

## Developing

```
$ docker-compose up -d
```

`$ docker-compose up -d`: 
- starts up a container for [Swagger UI](https://swagger.io/tools/swagger-ui/)
- starts up a container for [swagpack](https://www.npmjs.com/package/swagpack) to allows realtime build
- [Swagger UI](https://swagger.io/tools/swagger-ui/) can be accessed from http://localhost:3020
- DOES NOT supports HMR(Hot Module Replacement). Requires browser reload when you make changes to the spec file.

## How to publish
Pet Store API is hosted on [GitHub Package Registry](https://help.github.com/en/github/managing-packages-with-github-packages/about-github-packages).
Follow the instraction down below to publish latest version of the package privately.

- Generate personal access token from [here](https://github.com/settings/tokens/new). Minimum requisites is `repo`, `write:packages`, and `read:packages`.
- Run `$ echo "//npm.pkg.github.com/:_authToken=<YOUR ACCESS TOKEN>" >> ./.npmrc`
- Run `$ npm publish`
