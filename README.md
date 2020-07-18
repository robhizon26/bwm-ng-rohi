This is the finished code from the online training material [React, Angular, Node In-Depth Guide: Beginner to Pro (2020)](https://www.udemy.com/course/react-angular-node-in-depth-guide-beginner-to-pro-2020/) in Udemy by Filip Jerga. 

## See this app on Demo
This is running [live](https://bwm-ng-rohi.herokuapp.com/) hosted using Heroku.
 
## How to run this project

Create `dev.js` file in `server/config/dev.js` with content of:
```javascript
module.exports = {
  DB_URI: 'your_mongo_db_connection_string', // Get it here -> https://www.mongodb.com/
  JWT_SECRET: 'some_unique_value' // e.g: 'dasid7asd7xc68zxc!'
  CLOUDINARY_NAME: 'your_cloudinary_name', 
  CLOUDINARY_KEY: 'your_cloudinary_key', 
  CLOUDINARY_SECRET: 'your_cloudinary_secret'
}
```

Create `environments.ts` file in `/src/environments/environments.ts` with content of:
```javascript
export const environment = {
  production: false,
  TOMTOM_API_key: 'your_TOMTOM_API_key'
};
```
 

In base folder of project run `npm install` and then `npm start`

To run api server navigate to server folder `cd server` and run `node index.js`

## How to populate DB

In case your `dev.js` file is created you can run in `server` folder command to populate database `node fakeDB/cleanDB.js`

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

 