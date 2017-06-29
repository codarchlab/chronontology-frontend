# Chronontology (Frontend)

## Prerequisites

The following components need to be installed:
* [NodeJS](https://nodejs.org/)

## Installation of Dependencies

Install development and production dependencies with the following commands within your chronontology-frontend directory

```
npm install
```

## Configuration

```
cp dev-config.json.template dev-config.json
```

##  Running the development server

In order to run the frontend in the development server use the following command:
```
npm start
```

Chronontology frontend will access the backend on port 4567 and is accessible at [localhost:8085/](http://localhost:8085/). You can use a different backend instance by setting `backendUri` in `dev-config.json` (for example to http://chronontology.dainst.org/data in order to use the production backend).

Any changes made to HTML, SCSS or JS files should automatically trigger a browser reload.

##  Running the e2e tests

In order to run the e2e tests use the following command:
```
npm run e2e
```
The application has to be already running at [localhost:8085/](http://localhost:8085/): Either by running `npm start` in 
parallel or by deploying and serving a build at that address via your web-server of choice.

## Deployment

Build the application by running

```
npm run build
```

After building, chronontology-frontend lies inside the dist directory. 
