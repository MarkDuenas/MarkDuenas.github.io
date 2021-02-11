# Sending Form Data

`<form>` is used to send data to the server and is defined by two important attributes `action` and `method`

### Action attribute

Defines where the data gets sent. The value must be a valid relative or absolute URL.

`<form action="https://example.com">` - absolute URL
`<form action="/somewhere_else"> ` - relative URL

### Method attribute

Defines how data is sent. GET/POST method

**GET** method
  - method used by browser to ask server to send back a given resource.

**POST** method
  - method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request.

### Viewing HTTP requests
  - Open developer tools
  - Select "Nertwork"
  - Select "All"
  - Select "food.com" in the "Name" tab
  - Select "Headers"
