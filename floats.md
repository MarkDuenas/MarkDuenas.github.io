# CSS Floats
Source: [All About Floats](https://css-tricks.com/all-about-floats/)

## What is a float?

**Float** property applied to an element *remain a part of the flow of the web page*.
It makes elements wrap around the floated element. Meaning text will not overflow into an image or another element.

There are 4 valid values for float property: **Left**, **Right**, **None**, **Inherit**.
 - Left and Right float elements to those directions.
 - None makes the lement not float.
 - Inherit assumes the float value from the elements parent element.
 
## What are floats used for?

Aside from wrapping text around images, floats can create entire web layouts.

## Clearing the float

`clear` is float's sister property. If applied to an element it will not move adjacent to the floated element like it would normally do.
Instead it will move itself down past the float.

`clear` has 4 valid values: **Both**, **Left**, **Right**, **None**, **Inherit**.
  - Both commonly used. Clears floats coming from both directions.
  - Left and Right clears floats in the respective direction.
  - None is default.
  - Inherit technically the 5th one, but not supported on IE.
  
## The Great Collapse

If a parent element has elements that are all floated, this results in the parent element's height collapsing to nothing.
Collapsing always needs to be dealt with to prevent strange layout and cross-browser problems. To fix it, we clear the float
**after** the floated elements in the container but **before** the close of the container.

## Techniques for Clearing Floats

### The Empty Div Method
  - An empty div `<div style="clear: both;"></div>`.
  - Considered not semantic.
  
### The Overflow Method
  - Relies on setting the overflow CSS property on a parent element.
  - If set to *auto* or *hidden* on parent element, the parent will expand to contain the floats.

### The Easy Clearing Method
  - Uses CSS pseudo selector *:after* to clear floats.
  - Unlike overflow on the parent you apply the CSS like this:
  
  ```
  .clearfix:after { 
   content: "."; 
   visibility: hidden; 
   display: block; 
   height: 0; 
   clear: both;
  }
  ```
  - Applies a bit of content hidden from view, after the parent element which clears the float.
  
