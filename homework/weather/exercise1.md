# Homework 1 - The Weather Widget

* Example code from lecture 1 can be used as a basis.
* Make sure you understand what each piece that you do use is doing and pick
  only the part that are necessary to fulfil these requirements.
* Read through all the requirements carefully
* Ask any questions in the course Slack workspace

## Configure initial project (2 / 10 points)

* Create *index.html* 
  * Must include one JavaScript file (e.g /public/app.js) in document *head*
  * The JavaScript file must be executed after *DOM* has loaded
  * Set a *title* (_The Weather Widget_) to the document
* Specify ALL your dependencies in *package.json*
* yarn install && yarn build:watch must serve your application on localhost:10001
* yarn install && yarn test must lint your source files (including test/ folder) and run unit tests

## Building (3 / 10 points)

* Use Rollup as the build tool
  * Configure Rollup to output one JS file (e.g ./public/app.js)
  * Configure Rollup to use babel as a transpiler for JavaScript files
  * Configure Rollup to include source maps in the JavaScript bundle
* Configure Babel to output JavaScript that is
  * compatible with browsers with *equal to or more than 5% market share* according to browserlist
* Configure eslint
  * Configure to work with babel (_@babel/eslint-parser_)
  * Set "browser" as target environment
  * Use eslint and/or google recommended rules
  * Validate imports (_eslint-plugin-import_)
  * Lint your tests! (Create a different _eslint_ configuration file for the _test/_ folder)
* When localhost:10001 is open and any source file (not build configuration) is changed, the page should reload automatically.

## Unit tests (2 / 10 points)

* Use _jest_ as a test runner and an assertion framework
* ⚠️ Create at least 2 unit tests

## The Weather Widget (3 / 10 points)

* Should contain city name of your choice. E.g., Tartu
* Shoud contain a "Generate" button to update the following stats randomly:
  * Temperature: from -20°C to +30°C **inclusive**
  * Precipitation: one of ☀️, ⛅️, ☁️, 🌩️, 🌧️, 🌦️, 🌨️
  * Wind: from 0 km/h to 10 km/h **inclusive**
* Update weather stats every time when the button is clicked
* Align the elements to center with readable space in-between using flexbox
* Use h2 for the city name
* Use 2em as content font-size

## Style and submission

* For your own sanity, use a version control system (learn if you have to!).
* Use any editor of your liking, but don't include its configuration files in the submission
* Don't leave this to the last minute (really!)
* Don't include node_modules/ nor any other autogenerated files in your submission (also exclude them from source control)
* Make sure you have no JavaScript lint errors or warnings.
* Use CamelCase for variable, file and class naming (except CSS selectors).
* zip your files together (**don't include node_modules/, public/ - other than
  public/index.html - or .git/ or .hg/!**) and submit the zip file on the
  course submission page

## Pre-submission sanity check

* Delete node_modules/ directory and JavaScript and CSS files from the public/ directory
* Run yarn install && yarn lint && yarn test and check that your tests pass
* Run yarn build:watch and check that your application works as expected