# Reading Notes


## Code 301 Intermediate Software Development


### Responsive Web Design and Floats (SMACCS Pre-work)
Source: [RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/).

**RWD Overview**

- Responsive web design is the practice of building a website suitable to work on every device.

**Responsive vs. Adaptive vs. Mobile**

- Responsive generally means to react quickly to any change.
- Adaptive means to be easily modified for a new purpose or situation.
- Mobile generally means to build a seperate website commonly on a new domain soley for mobile users.

*Most popular technique lies within responsive web design*

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media.

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


