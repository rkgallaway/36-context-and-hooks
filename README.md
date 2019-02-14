![CF](http://i.imgur.com/7v5ASc8.png) LAB 36
=================================================

## Lab 36: Context and Hooks

### Author: Ryan Gallaway

### Links and Resources

[![Build Status](https://www.travis-ci.com/rkgallaway/36-context-and-hooks.svg?branch=master)](https://www.travis-ci.com/rkgallaway/36-context-and-hooks)
* [repo](https://github.com/rkgallaway/36-context-and-hooks)
* [travis](https://www.travis-ci.com/rkgallaway/36-context-and-hooks)
* [front-end](http://xyz.com) (when finished/applicable)

#### Documentation
* [swagger](http://xyz.com) (API assignments only)
* [jsdoc](http://xyz.com) (All assignments)

### Modules
#### `modulename.js`
##### Exported Values and Methods

## Before you begin
* Start with a new react app, created at Code Sandbox or locally with create-react-app

## Implement a Context Provider and Consumer
Create a React application that wraps the entire `<App/>` with a context provider, created using Context API. Then, create multiple components that act as consumers to your context, using it in various ways.

Specifically, build a counter that uses 3 separate components that subscribe to a common provider

### Requirements
* Create a Counter Provider component, which exposes the following state:
  * `count` - A number (default to 0)
  * `increment` - A reference to a function that increases the count
  * `decrement` - A reference to a function that decreases the count
* In the index.js, import CounterContext and wrap `<App />` in it, so that all child components can optionally subscribe to it as consumers.
* Your `<App />` component should simply pull in and render the following child components ...
* Create the following child components that register as a `.Consumer` to the provided context.
  * `<Incrementer />` - Renders a button that, when clicked, calls the `increment()` method in the `Counter Provider`
  * `<Decrementer />` - Renders a button that, when clicked, calls the `decrement()` method in the `Counter Provider`
  * `<Counter />` - Renders the current value of `count` from the Counter Provider
* Provide good styling. Use the css-in-js methodology within the components themselves.

### Testing
* Do a deep mount of the app, and set tests to make assertions on the child components that consume context from the Provider.
  * Can they see context?
  * Can they interact via published functions?
### Setup
#### `.env` requirements
* `PORT` - Port Number
* `MONGODB_URI` - URL to the running mongo instance/db

#### Running the app
* `npm start`
* Endpoint: `/foo/bar/`
  * Returns a JSON object with abc in it.
* Endpoint: `/bing/zing/`
  * Returns a JSON object with xyz in it.
  
#### Tests
*`npm test` to run tests?
* What assertions were made?
* What assertions need to be / should be made?

#### UML
![Context and Hooks UML](./assets/uml.jpg)  --this image hasn't been uploaded yet