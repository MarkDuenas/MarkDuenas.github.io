# Express

## PUT vs PATCH

[Source](https://rapidapi.com/blog/put-vs-patch/)

 - PUT is a method of modifying resource where the client sends data that updates the *entire* resource. It will overwirte the whole data being updated.
 - PATCH applies a partial update to the resource. It does not overwrite but only updates the spicific field you wish to update.
 
## Tools for "mock" API development

[PostMan](https://www.postman.com/features/mock-api/)

[MockServer](https://www.mock-server.com/)

[Nock](https://github.com/nock/nock)

## Swagger vs APIDocs.js

  - Swagger and APIDocs create documentation and version control for your APIs.
  - Swagger is more popular and easier to navigate due to having Swagger UI and Hub.
  
HTPP status code for successful API call:
  - 2xx ex.(201-208)

HTTP status code for unsuccessful API call:
  - 4xx ex.(400 Bad request)
  
## SOAP vs REST

[Source](https://stackify.com/soap-vs-rest/)

  - SOAP(Simple Object Access Protocol) exposes components of application logic as services rather than data.
  - REST(Representational State Transfer) operates through a solitary interface to access named resources. Used when exposing public API over the internet.
  
## Vocab

1. Web Server - or a system of one or more computers dedicated to running this software, that can satisfy client HTTP requests on the public World Wide Web
2. Express - minimal and flexible node.js application framework that provides many utilities such as HTTP methods for quick API access.
3. Routing - refers to how an application's endpoints responds to client requests.
4. WRRC - Web Request Response Cycyle. The way the modern web works. Client request is sent from browser to the server then the server sends a response back to client based on the clients request.

## Lecture Prep Readings

1. Which 3 things had you heard about previously and now have better clarity on?
  - Middleware is usually used on the request object to modify it in some way before it reaches the server.
  - Serving static files is a middleware that is part of express
  - TTD is a standard way of developing apps in the real world.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - Learn more about using MongoDB.
  - How to write effiecient tests for my app.
  - Connect to different databases using express.
  
3. What are you most excited about trying to implement or see how it works?
  - Custom middlewares for authentication.
