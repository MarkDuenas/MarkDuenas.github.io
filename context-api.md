# Context API

## Review, Research, Discussion

### Describe use cases for useMemo() and useReducer()

- useMemo() - returns memoized value. only computes values if the dependencies changed.
- useReducer() - alternative to useState. handle more complex states.

### Why do custom hooks need the use prefix?

For naming convention and easier to realize what the function is doing.

### What do custom hooks usually do?

used to call other hooks, or make a common task easier to reuse.

### Using any list of custom hooks, research and name one that you think will be useful in your applications

useForm() - to register inputs and handle form state easier.

### Describe how a hook that fetches API data might work

It could fetch the data and automatically break down the data you get back in smaller batches of data that you are able to use in your jsx.

## Vocab

- reducer - reducer function's returned value is assigned to the accumulator, whose value is remembered across each iteration throughout the array, and ultimately becomes the final, single resulting value
