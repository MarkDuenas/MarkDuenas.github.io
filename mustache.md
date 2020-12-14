# Templating using Mustache.js
Souce: [Mustache.js](https://medium.com/@1sherlynn/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2)

## JavaScript Templating

JS templating is a fast and efficient technique to render client-side view templates with JS by using JSON data source.
Template engine replaces variables and instances declared in a template file with actual values at runtime.

## Mustache

Mustache is a logic-less template syntax. It is "logic-less" becahse there are no if statements, else clauses, or for loops.
Instead they use HTML tags.

Mustache syntax:

```
Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn
```

  - {{name}} is mustache syntax that acts as place holders for variables you want to pass to the html.
  
