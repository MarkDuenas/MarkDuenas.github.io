# Hooks API

## Review, Research, and Discussion

### Why do we not need more .html pages in a multi-page React app?

Because we insert all of the react code inside the index.html after it is all compiled.

### If we wanted a component to show up on every page, where would we put it and why?

Inside the `<BrowserRouter />`, outside a `<Route />` because everything inside the Route tag only shows up on the specific route.

### What does props.children contain?

It contains all the components that are inside a parent component tag.

## Vocab

- Composition - a way to combine objects or data types into more complex ones.
- Children / Child Components - Anything that is inside a opening and closing parent component JSX tag.
- Hash Routing -  using the anchor part of the URL to simulate different content.
- Link Routing - every node constructs a map of the connectivity to the network, in the form of a graph, showing which nodes are connected to which other nodes.
