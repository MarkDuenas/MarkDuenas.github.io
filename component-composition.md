# Component Composition

## Review, Research, and Discussion

### Can a parent component access the state of a child component?

- Not directly. If a function is created on the Parent component that returns something and passed down to the child component, 
the child component can then call the passed down function and return whicever state the parent component needs.

### What can be passed along in a prop variable?

- Functions and states.

### How can a child component “know” the state of another component?

- by having state on the parent component and passed down to both child components.

## Term

- component props - Props are arguments passed into React components.
- component state - The state object is where you store property values that belongs to the component. When the state object changes, the component re-renders.
- application state - An application state is simply the state at which an application resides with regards to where in a program is being executed and the memory that is stored for the application.
