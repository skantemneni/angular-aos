# AngularAos

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.2.12.

Here are teh steps we used to Generate and add AOS to this Angular project.

### 1.)  ng new angular-aos --style scss --routing true
cd angular-aos/

installing the Animate On Scroll (AOS) library.
npm install aos
npm i --save-dev @types/aos
(Optional) npm install --save @types/aos


### 2.) update the styles array in the angular.json
Angular.json From ---> To

            "styles": [
              "src/styles.scss"
            ],

            "styles": [
              "src/styles.scss",
              "node_modules/aos/dist/aos.css"
            ],

### 3.) Initializing/ Animating with the Animate On Scroll Library (AOS).
import * as Aos from 'aos';

### 4.) init() function in the ngOnInit of our component.ts
Aos.init();

### 5.) Test from component.html

<div data-aos="fade-up" data-aos-duration="3000">
  Lord Shiva is Great!!!
</div>




## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
