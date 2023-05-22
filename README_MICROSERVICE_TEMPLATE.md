![Logo](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

# Project Title

A brief description of what this project does and who it's for.

This is the resource API for [placeholder](https://github.com/sample) data in dynamodb.

## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![Build status](https://badge.buildkite.com/6bb74d6ed14df31518a3feeb047fe9c6c7d13bedf2bece76c1.svg?branch=master)](https://buildkite.com/<api_name>)

![Architecture design](https://via.placeholder.com/468x300?text=Architecture+Design+Here)


This API runs at:

- [local](http://localhost:8080/<api_name>)
- [staging](https://<api_name>.staging.cloud.acme.com.au/health)
- [prod](https://<api_name>.cloud.acme.com.au/health)

## Custodian

- Team:
- SLA: Australian Business Hours

## Development

The main tech stack of this project is Typescript, AWS DynamoDB SDK and CloudRun

<a id="markdown-prerequisites" name="prerequisites"></a>

### Prerequisites

- [node](https://nodejs.org/en/)
- [yarn](https://yarnpkg.com/en/docs/install#mac-stable)
- [docker](https://docs.docker.com/docker-for-mac/install/)

### Get started

To get started, checkout the repo and run

```bash
yarn
```

Start server

```bash
yarn start #API runs at http://localhost:8080/health
```

Run test

```bash
yarn ci
```

Pre check in your code

```bash
yarn pre-checkin
```

Run local E2E test

```bash
export NPM_TOKEN=xxxx   # or set this environment variable in your profile

yarn run:local:e2e
```

For other commands, please refer to [package.json](https://github.com/<repo_name>/blob/master/package.json#L8);

### Postman collection

You can use the postman collection to run some manual tests for the endpoints.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/<uuid>)

You need to create an **Environment** with the following variables

- base_url
- id_token
- env

## Monitoring and alerting

### Splunk

- [staging](https://acme.splunkcloud.com/en-US/app/search/search?q=<query>)
- [prod](https://acme.splunkcloud.com/en-US/app/search/search?q=<query>)

### Pagerduty

Alarms is sent to [Team Business Hours](https://acme.pagerduty.com/services/<id>)

### Datadog APM (or could be appdynamics here)

- [dev](uri)
- [prod](uri)

## Dependabot

> Dependabot is used to keep all our dependencies up to date

## Contributing

Contributions are always welcome!

See `contributing.md` for ways to get started.

Please adhere to this project's `code of conduct`.

## Resources

- [Team tech docs](uri) -- each team could have their own tech docs using mkdocs similar to spotify backstage approach
- [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
- [Awesome README](https://github.com/matiassingers/awesome-readme)
- [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)
- [JVM microservice guide](https://blog.shanelee.name/2017/07/15/jvm-microservice-with-spring-boot-docker-and-kubernetes/)
