# Node.js

## What is Node.js?

Description:
- Node.js is a JavaScript runtime built on Chrome's V8 JavaScript engine.

## Node is built on Google Chrome's V8 JS Engine.

- The V8 engine is the open-source JS engine that runs in Google Chrome.
- Designed with performance in mind and responsible for compiling JS directly to native machine code that your computer can execute.
- Node programs does not execute in a browser.
- Creator of Node took the V8 engine and enchanced it with more features.
- Node.js is a program we can use to execute JS on our computers(JS runtime).

## How Do I Install Node.js?

### Node Binaries vs Version Manager

- Using a version manager allows you to install and swap between different Node versions at will.


## Node.js Has Excellent Support for Modern JavaScript

- Can write the latest and most modern syntax of JS.
- Generally don't have to worry about compatibility issues as you would if you were writing JS that would run in different browsers.

## Introducing npm, the JS Package Manager

Node comes bundled with a package manager called npm.
Npm is also the world's largest software registry.

### Installing a package globally

`npm install -g jshint`
  - the -g installs it globally.

### Installing a package locally

`npm init -y`
  - create and autopopulate a `package.json`

## What is Node.js Used For?

- We can use node to run various tools we install with npm.
- Many modern front-end framework use Node to run npm packages.

## Node.js Let's Us Run JS on the Server

### The Node.js Execution Model

- Node.js is single-threaded
- It's event-driven which means that everything that happens in Node is in reaction to an event.
- Under the hood Node uses the libuv library to implement this asynchronous(that is, non-blocking) behaviour.
- Capable of handingling a large number of simultaneous connections.

