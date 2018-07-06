# Starter-pack

<!-- TOC -->

- [Starter-pack](#starter-pack)
    - [Summary:](#summary)
    - [I - Make it work 👍](#i---make-it-work-👍)
        - [1. Install dependencies:](#1-install-dependencies)
        - [2. Install gulp *( in global )*:](#2-install-gulp--in-global-)
        - [3. Build and / or watch:](#3-build-and--or-watch)
    - [II - Create new scss and js files](#ii---create-new-scss-and-js-files)
        - [1. Tree](#1-tree)
        - [2. To create new components files:](#2-to-create-new-components-files)
            - [SCSS](#scss)
            - [JS](#js)
    - [III - Dependencies](#iii---dependencies)

<!-- /TOC -->
## Summary:
* I - Make it work
    * 1. Install dependencies
    * 2. Install gulp ( in global )
    * 3. Build and / or watch
* II - Create new scss and js files
    * 1. Tree
    * 2. To create new components files
        * SCSS
        * JS
* III - Dependencies
## I - Make it work 👍
### 1. Install dependencies:
* use `yarn` or `npm install`

### 2. Install gulp *( in global )*:
* use `yarn global add gulp` or `npm install -g gulp`

### 3. Build and / or watch:
* use `gulp build` to build your work **one time**
* or simply `gulp` to build it **in a loop** and actualize your modifications

> Now you have your environment **ready to work**

## II - Create new scss and js files

### 1. Tree

```bash

├── public
│   ├── index.html
│   ├── assets
│   │   ├── fonts
│   │   └── images
│   ├── css
│   │   └── master.min.css
│   └── js
│       └── app.min.js
├── src
│   ├── js
│   │   ├── app.js
│   │   └── ui.js
│   └── scss
│       ├── components
│       │   ├── _footer.scss
│       │   └── _header.scss
│       ├── global
│       │   ├── _fonts.scss
│       │   ├── _global.scss
│       │   ├── _reset.scss
│       │   └── _variables.scss
│       ├── mixins
│       │   └── _responsive.scss
│       └── master.scss
├── .babelrc
├── .gitignore
├── .jshintrc
├── gulpfile.js
├── package.json
├── README.md
└── yarn.lock
```

### 2. To create new components files: 

#### SCSS

* Go to `src/scss/components`
* Create your file with this structure: `_filename.scss` 
+ Don't forget to import this new file in `master.scss` like that: `@import: 'component/filename'`

#### JS 

* Go to `src/js`
* Create your file with this structure: `filename.js` 
+ Don't forget to import this new file in `app.js` like that: `import: './filename'`

## III - Dependencies

```json
    "babel": "^6.23.0",
    "babel-core": "^6.26.3",
    "babel-preset-es2015": "^6.24.1",
    "browser-sync": "^2.24.4",
    "gulp": "^3.9.1",
    "gulp-babel": "^7.0.1",
    "gulp-rename": "^1.3.0",
    "gulp-sass": "^4.0.1",
    "gulp-uglify-es": "^1.0.4",
    "jshint": "^2.9.5",
    "webpack-stream": "^4.0.3"
```
```bash
.jshintrc
```