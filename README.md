# JugTour FrontEnd


**Description:**  

Getting started with the front end of the application by setting up the UI using React app.

**Pre-requisites:**

[yarn](https://yarnpkg.com/en/docs/install#mac-stable) should be installed.


## Getting Started
To create the React UI, first create a new project in the `jugtours` directory with yarn:
```
yarn create react-app app
```
Navigate to the `app` directory and install [Bootstrap](https://getbootstrap.com/), cookie support for React, React router and [Reactstrap](https://reactstrap.github.io/) using yarn:
```
cd app
yarn add bootstrap@4.1.3 react-cookie@3.0.4 react-router-dom@4.3.1 reactstrap@6.5.0
```
Add Bootstrap's CSS file as an import in `app/src/app.js`:
```
import 'bootstrap/dist/css/bootstrap.min.css';
```
To call the Spring Boot API `/api/groups`, modify the App.js in `app/src/App.js` and replace it with [this](https://github.com/samujjal1618/JugTourFrontEnd/blob/master/app/src/app.js).

To proxy from `/api` to `http://localhost:8080/api`, add a proxy setting to `app/package.json`:
```
"scripts": {...},
"proxy": "http://localhost:8080",
```
To start the application run `yarn start` in the `app` directory.



