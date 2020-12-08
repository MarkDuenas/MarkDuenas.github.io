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
  
### Updating Elements

All methods used as setters(updates element)

`.html()`
  - gives every element retrieved the same content, can include HTML tags.
  
`.text()`
  - gives every element same new text content, markup will be shown as text.
  
`.replaceWith()`
  - replace every element with new content, also returns replaced elements.
  
`.remove()`
  - removes all of the elements in the matching set.

*.html(), .text(), .replaceWith() can take strings as parameters*

### Inserting Elements

  1. Create new elements in jQuery.
    - `var $newFragment = $('li');` this creates a jQuery object that contain an empty `<li>` element.
    - Can also do `var $newItem = $('<li class="new"> item </li>');`
  
  2. Adding new elements to page.
    - `.before()` and `.after()` inserts content before/after elected elements(s).
    - `.prepend()` and `.append()` inserts content ***inside*** the selected elements(s) after opening tag/before closing tag respectively.
    
  

### Getting and Setting Attribute Valus

  `.attr()`
    - get/set specified attribute and its value ex. `$('li#one').attr('id');`
  
  `.removeAttr()`
    - removes specified attributes. `$('li#one').removeAttr('id');`
    
  `.addClass()` and `.removeClass()`
    - adds/removes value to existing value of the class attribute.
    
### Getting and Setting CSS Properties

  `.css()` method lets you retrieve and set the values of CSS properties.
  
  1. To get a CSS property of an element
    - `var = backgroundColor = $('li').css('background-color');`
  
  2. To set a CSS property, pass in a secon argument.
    - `$('li').css('background-color', 'blue');`
    
### Working with each element in a selection

jQuery uses `.each()` method to loop through a selection of elements.

```
$('li').each(function() {
  var ids = this.id;
  $(this).append('<em class='order'> + ids i '</em>');
});
```
`.each()` applies the same code to each element in the selection.

### Event Methods

The `.on()` method is used to handdle all events.

`.on()` method takes two parameters, first parameter is the event and the second is the code you want to execute once the event has been met.

Example:

```
$('li').on('click', function() {
  $(this).addClass('complete');
});
```

### Event Object

Every event handling function receives an event object.

```
$('li').on('click', function(event) {
  eventType = event.type;
});
```

***event*** is the event object parameter give a anem of *event*.



    

