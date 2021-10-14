# Express Backend Quickstart Guide

## Assumptions
- npm installed
- app folder created, which will contain frontend & backend folders
- mongoose as our database (this could be replaced by postgresql, nosql, etc.)

## Installation & Setup
1. create backend folder: mkdir backend
2. go to backend folder: cd backend
3. create package.json & package-lock.json files: npm init
4. install packages: npm install cors express mongoose validator requests
5. install developer packages: npm i -D nodemon
6. create a .gitignore file to exclude node_modules: echo /node_modules > .gitignore

## Express Server setup
1. create an index.js file... and in that file:
  - const express = require("express");
  - const app = express();
  - app.get("/", (req, res) => res.send("This Works"));
  - const port = process.env.PORT || 5000;
  - app.listen(port, () => console.log(`Server is up on port ${port}`));
 2. to keep routes less complicated, and for when it gets complicated, create a routes/api folder: mkdir routes/api
 3. go to routes/api folder: cd routes/api
 4. create first routes file: touch _first_routes_file_... and in that file:
  - const express = require("express");
  - const router = express.Router();
  - import any data models
  - router.get('/', (req, res) = {..._do_something_here_...});
  - module.exports = router;
 

## Database setup
1. create a models folder: mkdir models
2. To-be-done...
