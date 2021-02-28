# Express REST API

1. Name 3 real world use cases where you’d want to change the request with custom middleware
  - Authentication of user.
  - Hashing password for user.
  - Timestamps

2. True or false: The route handler is middleware?
  - false

3. In what ways can a middleware function end the process and send data to the browser?
  - by using the next() function passed through the middleware.

4. At what point in the request lifecycle can you “inject” middleware?
  - During the initial request from client to server.

5. What can cause express to error with “Request headers sent twice, cannot start a second response"
  - Sending another response to the client after a response has already been sent.

## Vocab

1. Middleware - Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle.
2. Request Object - The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.
3. Response Object - The res object represents the HTTP response that an Express app sends when it gets an HTTP request.
4. Application Middleware - App wide middleware that's used once and active all the time.
5. Routing Middleware - Route level middleware triggers when the specific route it's attached to is activated.
6. Test Driven Development - A development practice that writes test's based on software requirements of the app before the actual code is written for the app.
7. Behavioral Testing - An extension of TDD. A development practice that encourages collaboration among developers in a software project.
