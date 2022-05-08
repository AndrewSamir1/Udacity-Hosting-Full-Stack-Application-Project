# Hosting a Full Stack Application

## Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

## Pipeline Process

### Continuous Integration

#### GitHub

GitHub Repository is used to store code and to be trigger CircleCI automated process.

#### CircleCI

CircleCI uses the configuartion file to know the scripts to be ran. We have to scripts here, one for building and deploying the frontend,
and the other for building and deploying the backend.

## Front End Scripts

- Build the code.
- Upload built folder to S3 Bucket

## Back End Scripts

- Build the code.
- Upload built folder to EBS Enviroment.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework
