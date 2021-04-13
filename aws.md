# AWS: Cloud Servers

## Review, Research, and Discussion

### What’s the difference between a FIFO and a standard queue?

FIFO queues provide additional features that help prevent unintentional duplicates.

### How can the server be assured a message was properly received?

Have the client emit a received message to confirm on the server side.

### What classic design pattern is best represented by event driven programming?

Observer Pattern: a behavioral design pattern that lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.

### How do you test an event driven system?

Unit testing the function helpers.

## Vocab Terms

1. Server - is a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients".
2. Pub/Sub - is an asynchronous messaging service that decouples services that produce events from services that process events.
3. WRRC - web request response cycle. Clients requests info from servers then servers respond by send info back to their browser.
