## Making an App with Angular 8

### Created by Angelo Osorio


### Notes:
#### To install bootstrap on a project

1. Install bootstrap
- npm i bootstrap

2. Install requirements to bootstrap
- npm i jquery popper.js

3. Edit project-name/angular.json:
```javascript
"styles": [
   ...
   "node_modules/bootstrap/dist/css/bootstrap.min.css"
],
"scripts": [
   ...
   "node_modules/jquery/dist/jquery.min.js",
   "node_modules/popper.js/dist/umd/popper.min.js",
   "node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```