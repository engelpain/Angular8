## Making an CRUD App with Angular 8 and firebase
### Created by Angelo Osorio



### Index
1. [Requirements](#1-requirements)
1. [Create a project](#2-create-a-project)
1. [Create a component](#3-create-a-component)
1. [Create a service](#4-create-a-service)
1. [Notes]()

### 1. Requirements:
- NodeJS v10.16.0
- npm v6.10.0
- Angular V8

#### Installing Angular
- install Angular CLI on Global
   * ```npm install -g @angular/cli```



### 2. Create a project
- Create project:
   * ```ng new project-name```

- Run project:
   * ```ng serve```



### 3. Create a component
- Generate a component:
   * ```ng generate component component-name```
- You also can use the shorthand:
   * ```ng g c component-name```



### 4. Create a service
- Generate a service:
   * ```ng generate service service-name```
- You also can use the shorthand:
   * ```ng g s service-name```

- If you want to place a new service in a folder, you can use this code:
   * ```ng generate service folder-name/service-name```
- Or also:
   * ```ng g s folder-name/service-name```

After generate a service, you need to add it on *app.module.ts*, because this is not done for you
automatically like the components.

- Adding services to app:
   - Open *app.module.ts*, after all previous imports, introduce the following code:
```TypeScript
...
import { ServiceNameService } from "./service-name.service";
```

   - Open *app.module.ts*, after all previous imports, introduce the following code:
```TypeScript
...
providers: [ServiceNameService]
```

### 5. Add your component to app root
- Open *app.component.html* and add the new component:

```html
   <app-orders></app-orders>
```

### Notes:
#### To install bootstrap on a project

1. Install bootstrap:
   - `npm i bootstrap`

2. Install requirements to bootstrap:
   - `npm i jquery popper.js`

3. Edit project-name/angular.json:
   - On line 27 add bootstrap:
```javascript
"styles": [
   ...
   "node_modules/bootstrap/dist/css/bootstrap.min.css"
],
```
```javascript
"scripts": [
   ...
   "node_modules/jquery/dist/jquery.min.js",
   "node_modules/popper.js/dist/popper.min.js",
   "node_modules/bootstrap/dist/js/bootstrap.bundle.min.js"
]
```

### To install fontawesome on a project

1. Install fontawesome
   - ` npm i @fortawesome/fontawesome-free`


2. Edit project-name/angular.json:
   - On line 27 add fontawesome:
```javascript
"styles": [
  ...
  "node_modules/@fortawesome/fontawesome-free/css/all.min.css"
],
```
```javascript
"scripts": [
  ...
  "node_modules/@fortawesome/fontawesome-free/js/all.min.js"
]
```