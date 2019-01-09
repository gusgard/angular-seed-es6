
# angular-seed-es6

[![Build Status](https://travis-ci.org/gusgard/angular-seed-es6.svg)](https://travis-ci.org/gusgard/angular-seed-es6)
[![devDependency Status](https://david-dm.org/gusgard/angular-seed-es6.svg)](https://david-dm.org/gusgard/angular-seed-es6#info=devDependencies)

This project is an application skeleton for a typical [AngularJS 1.x](http://angularjs.org/) web app using the [best practices](https://github.com/johnpapa/angular-styleguide/blob/master/a1/README.md) and with **ES6**.
You can use it to quickly bootstrap your angular webapp projects and dev environment for these
projects.

The seed contains a sample AngularJS application and is preconfigured to install the Angular
framework and a bunch of development tools for instant web development gratification.

The seed app doesn't do much, just shows how to wire two controllers and views together.

## Features

Please see the [gulpfile](./gulpfile.babel.js) for up to date information on what it supports.

* ES6 out of the box
* Browserify
* Built-in hot-reload preview server with BrowserSync
* Compile Sass with [libsass](http://sass-lang.com/libsass)
* Map compiled JS/CSS to source with source maps
* HTML and CSS minification
* Cache-busting to all JS and CSS files


## Getting Started

- Install dependencies: `npm install`
- Run `npm start` to preview and watch for changes with hot reload
- Run `npm run build` to generate a distributable, production-ready, `build` directory

Now browse to the app at `http://localhost:8000`.

## Directory Layout for development

```
app/                    --> all compiled files for the application
  assets/               --> static files
    favicon.ico
  js/                   --> js files
    view-one/
      controllers/
        controllers.js    --> controller logic
      services/
        count-store.js    --> service logic
      directives/
        title-example.js  --> directive logic
      modules.js          --> define the module dependencies
    view-two/
      controllers/
        controllers.js    --> controller logic
      modules.js          --> define the module dependencies
    modules.js            --> main application module, load all states for the page.
  scss/                   --> sass files
    section/
      view-one/
        _index.scss
      view-two/
        _index.scss
        count-store.js
    variables/
      _colors.scss
      _index.scss
    main.scss           --> main sass
  templates/            --> html files
    view-one/
      view-one.html
    view-two/
      view-two.html
  index.html            --> the main html template file of the app
```


## Directory Layout  for production

```
build/                  --> all compiled files for the application
  assets/               --> static files
    favicon.ico
  css/                  --> css files
    main.min.css        --> compiled scss
    main.min.css.map    --> source map for scss
    libs.min.css        --> compiled third-party styles
    libs.min.css.map    --> source map for third-party styles
  js/                   --> js files
    app.js              --> minify angular files
    libs.js             --> minify third-party librarys
  templates/            --> html files
    view-one/
      view-one.html     --> minify html
    view-two/
      view-two.html     --> minify html
  index.html            --> the main html template file of the app
```
## Testing

* TODO

## Inspired by
- [angular-seed](https://github.com/angular/angular-seed)
