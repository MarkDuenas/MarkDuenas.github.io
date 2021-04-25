# AWS: Events

## Review, Research, and Discussion

### What’s the difference between a FIFO and a standard queue?

FIFO queues provide additional features that help prevent unintentional duplicates.

### How can the server be assured a message was properly received?

Have the client emit a received message to confirm on the server side.

### What classic design pattern is best represented by event driven programming?

Observer Pattern: a behavioral design pattern that lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.

### How do you test an event driven system?

Unit testing the function helpers.

## Vocab Term

- Serverless API - A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider.
- Triggers - an event or something similar that will execute the respective function(lambda function).
- Dynamo vs Mongo - DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas. DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents.
- Dynamoose vs Mongoose - Dynamoose works with DynamoDB and Mongoose with Mongo. They are essentially the same with different syntax on queries.
