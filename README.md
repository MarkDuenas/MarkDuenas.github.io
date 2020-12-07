# Reading Notes


## Code 301 Intermediate Software Development
[All About Floats](./floats.md)

### Responsive Web Design and Floats (SMACCS Pre-work)
Source: [RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/).

**RWD Overview**

- Responsive web design is the practice of building a website suitable to work on every device.

**Responsive vs. Adaptive vs. Mobile**

- Responsive generally means to react quickly to any change.
- Adaptive means to be easily modified for a new purpose or situation.
- Mobile generally means to build a seperate website commonly on a new domain soley for mobile users.

*Most popular technique lies within responsive web design*

Responsive web design is broken down into three main components, including ***flexible layouts***, ***media queries***, and ***flexible media***.

**Flexible Layouts**

- The practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.
- Built using relative length units (percentages or em units).
- Does not use fixed measurement units (pixels or inches). Fixed values have too many constraints.
- Formula for relative width of target element 
  - `target ÷ context = result`

*Flexible Grid*

Without using the flexible grid formula:

HTML
```
<div class="container">
  <section>...</section>
  <aside>...</aside>
</div>
```
CSS
```
.container {
  width: 538px;
}
section,
aside {
  margin: 10px;
}
section {
  float: left;
  width: 340px;
}
aside {
  float: right;
  width: 158px;
}

```

Using the flexible grid formula:

```
section,
aside {
  margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */
}
section {
  float: left;
  width: 63.197026%;    /* 340px ÷ 538px = .63197026 */   
}
aside {
  float: right;
  width: 29.3680297%;  /* 158px ÷ 538px = .293680297 */
}
```
**Media Queries**

Provide the ability to speciafy different styles for individual browser and device circumstances, such as the width of the viewport.

*Initializing Media Queries*

- Can be used in multiple ways 
 1. @media inside an existing style sheet.
  
```
 <!-- Separate CSS File -->
 <link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">
```

  2. @import a new style sheet.

```
/* @import Rule */
@import url(styles.css) all and (max-width: 1024px) {...}
```

  3. linking to a seperate style sheet from within HTML document.
  
```
/* @media Rule */
@media all and (max-width: 1024px) {...}
```

*Logical Operators in Media Queries*

Three different logical operators: ***and***, ***only*** and ***only***.

- Using ***and*** logical operator allows extra conditions to be added and met.
  - Ex. `@media all and (min-width: 800px) and (max-width: 1024px) {...}`

- The ***not*** logical operator specifies any query but the one identified.
  - Ex. `@media not screen and (color) {...}`
  
- The ***only*** logical operator triggers only if the specified condition is met.
  - Ex. `@media only screen and (orientation: portrait) {...}`
  
*Media Feautures*

1. Height and Width
  - Based off the height and width of the viewport rendering area(browser window).
  - Values can be any length unit, relative or absolute.
  `@media all and (min-width: 320px) and (max-width: 780px) {...}`
2. Orientation Media
  - Determines if device is in landscape or portrait.
  `@media all and (orientation: landscape) {...}`
3. Aspect Ratio
  - Specifies the width/height pixel ratio of the rendering area.
  `@media all and (min-device-aspect-ratio: 16/9) {...}`
4. Resolution
  - Specifies resolution of output deivce in pixel density(DPI)
  `@media print and (min-resolution: 300dpi) {...}`

**Mobile First**

Mobile first approach includes using styles targeted at smaller viewports as the default style, then use
media queries to add styles as the viewport grows.

```
@media screen and (min-width: 400px)  {...}
@media screen and (min-width: 600px)  {...}
@media screen and (min-width: 1000px) {...}
@media screen and (min-width: 1400px) {...}
```

**Viewport**

Apple invented viewport meta tag to help mobile devices identify the viewport size, scale and resolution of a website.

*Viewport Height and Width*

For the best results, and the best looking website, it is recommend that you use the device defaults by applying the device-height and device-width values.

`<meta name="viewport" content="width=device-width">`

*CSS Viewport Rule*
> Since the viewport meta tag revolves so heavily around setting the styles of how a website should be rendered it has been recommend to move the viewport from a meta tag with HTML to an @ rule within CSS. This helps keep the style separated from content, providing a more semantic approach.
Currently some browsers have already implemented the @viewport rule, however support isn’t great across the board. The previously recommended viewport meta tag would look like the following @viewport rule in CSS.

```
@viewport {
  width: device-width;
  zoom: 1;
}

```

**Flexible Media**

Images, videos and other media types needs to be scalable as viewport changes.

Using `max-width` property with a value of `100%` ensures the media will scale down acccording to its containers width.

*Flexible Embedded Media*

The `max-width` property doesn't work for all intances, such as iframes and embedded media.

To get embedded media to be fully responsive the element needs to be absolutely positioned within a parent element.
The parent elemnet needs to have a `width` of `100%` so it will scale based on width of the viewport.

Parent element also needs to have a `height` of `0` to trigger the `hasLayout` within Internet Explorer.




  




