# Login and Auth

## Review, Research and Discussion

### Why is the Context API useful?

 It's a way for a React app to effectively produce global variables that can be passed around
 
### Can a component outside of a provider get its context?

Yes it can grab anythiang from context.

### What are some common use cases for using the Context API?

Theme of the app, login, authentication.

### Describe “Context Hell”

Putting too many state in context and handling them in context instead of at the component level.

## Vocab

- global state - state that is available throughout the whole application
- global context - context that wraps around the whole app, making state available to use.
- provider - a component that wraps around other components that want to use a global state.
- consumer - a component that uses anything from context.
