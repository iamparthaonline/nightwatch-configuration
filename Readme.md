# Setup for End to End flow testing using Nightwatch JS

This is a setup for [`Nightwatch.js`][man] for performing End-to-End tests in Node.js quickly and effortlessly that run against a Selenium/WebDriver server.

For more information about how `Nightwatch` APIs work, and how to use them,
the following resources are a great place to start:

- The [API reference][api] of Nightwatch.
- The [Developer Guide][help] on the Official site.
- [Learn Nightwatch][learn]
- UI Testing with Nightwatch.js — [Page Objects][pageobjects]
- [Nightwatch.js Gotchas][gotchas]
- [Nightwatch how to assert multiple elements][multi]



[man]: http://nightwatchjs.org/
[help]: http://nightwatchjs.org/guide
[api]: http://nightwatchjs.org/api
[learn]: https://github.com/dwyl/learn-nightwatch
[pageobjects]: http://matthewroach.me/ui-testing-with-nightwatch-js-page-objects/
[gotchas]: https://ericheikes.com/nightwatch-js-gotchas/
[multi]: https://stackoverflow.com/questions/27116103/nightwatch-js-how-to-assert-multiple-elements?rq=1

## Folder structure

- the root folder contains the main [`configuration`](./nightwatch.conf.js) file. 
- [`Tests`](./tests) contains testcases for various features.
- [`Reports`](./reports) contains the reports for the tests. 

## System Requirements
- Node js
- Java
- Selenium Web driver
- Browser specific Web drivers

## Installation

npm install --save-dev nightwatch

npm install --save-dev selenium-server

npm install --save-dev chromedriver geckodriver

Configuration file - http://nightwatchjs.org/gettingstarted/#settings-file

## Running Test cases 

### Running all the 
nightwatch -c nightwatch.conf.js -e chrome,firefox

### Running specific test case
nightwatch -c nightwatch.conf.js -e chrome --test tests/features/google.test.js


** tests/nightwatch.conf.js – the configuration for the test



