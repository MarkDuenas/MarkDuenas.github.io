# Props and State

## Review, Research, and Discussion

### Does a deployed React application require a server?

No it does not require a back-end server.

### Why do we prefer to test a React application at the behavior rather than the unit level?

Because it's hard to access the functions inside a component.

### What does npm run build do?

It compiles all the jsx into html, css, js files into a build folder and that is what gets deployed.

### Describe the actual composition / architecture of a React application

React creates an index.html and a index.js and an component call App.js. App.js gets push into the index.html root div and gets rendered that way. Babel converts jsx into regular JS.

## Terms

- BDD - Behaviour-Driven Development is a collaborative approach to software development that bridges the communication gap between business and IT.
- Acceptance Tests - a testing technique performed to determine whether or not the software system has met the requirement specifications.
- mounting - Mounting is the phase in which our React component mounts on the DOM (i.e., is created and inserted into the DOM).
- build - npm run build creates a build directory with a production build of your app. 
