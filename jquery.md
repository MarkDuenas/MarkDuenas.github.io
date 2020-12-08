# jQuery, Events, and the DOM

Source: *JavaScript and jQuery book by Jon Duckett pages 293-301, 306-331 and 354-357*

## What is jQuery?

**jQuery** is a JavaScript file that you inclued in your web pages.
Allows you to find elements using CSS-style selectors and then use jQuery methods to interact with them.

### Find elements using CSS-Styly selectors

  - Function jQuery() enables you to find elements in the page.
  - jQuery() creates an object called jQuery(holds reference to the element).
  - `$()` used as shorthand for jQuer().
  - `$('li.hot')` takes a CSS-selector as parameter.
  
### Do something with the element using jQuery methods

`$('li.hot').addClass('complete');`
  - `$('li.hot')` creates object based on the element selected
  - `.addClass('complete');` method used on the created object and updates the element.


## Why use jQuery?

  1. Simple selectors
    - Compatible across all browsers due to its use of CSS selectors.
  2. Common tasks in less code
    - Simplifies tasks such as looping through elements while using less code.
    - Chaining of methods
  3. Cross-browser compatibility

## jQuery Methods

### Getting Element Content

`.html()`
  - retrieves *only* the HTML inside the *first* element in the matched set.

`.text()`
  - will return content(text only, without html) from *every* element in the jQuery selector, along the text from any decendants.
  
### Getting at Content

