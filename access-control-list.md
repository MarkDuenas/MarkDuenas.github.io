# ACL

## Basic Authorization vs Bearer Authorization

Basic Auth - lets you access API/routes/websites using user credentials such as username/password.

Bearer Auth - uses a generated token to verify if that user has access to the specific information in the route.

## JSON Web Token

JWT package - lets you create/sign JWT with the user information along with a secret passcode that will get encoded and passed back to the client to be used as authentication.

## Storing a secret

Consider storing it in a .env file, and dont push it to your database.

## Vocab Term

- Ecnryption - the method by which information is converted into secret code that hides the information's true meaning.
  The science of encrypting and decrypting information is called cryptography.
- token - an Internet proposed standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims.
- bearer - Bearer authentication (also called token authentication) is an HTTP authentication scheme that involves security tokens called bearer tokens.
- secret - secret keyword passed in with user info to create.
- JSON Web Token - token that is made from user and a secret and sent to the browser.
