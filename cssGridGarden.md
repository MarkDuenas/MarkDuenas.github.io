# CSS Grid
Source: [CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

CSS Grid Layout (aka “Grid”), is a two-dimensional grid-based layout system that aims to do nothing less than completely change the way we design grid-based user interfaces.


### display
Defines the element as a grid container and establishes a new grid formatting context for its contents.

Values:
  - grid - generates a block-level grid
  - inline-grid - generates an inline-level grid
  
```
.container {
  display: grid | inline-grid;
}
```

### grid-template-columns | grid-template-rows
Defines the columns and rows of the grid with a space-separated list of values.

Examples:
```
.container {
  grid-template-columns: 40px 50px auto 50px 40px;
  grid-template-rows: 25% 100px auto;
}
```

If your definition contains repeating parts you can use `repeat()`

The `fr` unit allows you to set the size of a track as a fraction of the free space of the grid container.

```
.container{
  grid-template-columns: 1fr 1fr 1fr;
}
```

### grid-template
Shorthand for setting grid-template-rows, grid-template-columns and grid-template-areas.

```
.container {
  grid-template: none | <grid-template-rows> / <grid-template-columns>;
}
```

### column-gap | row-gap
Specifies the size of the grid lines. You can think of it like setting the width of the gutters between the columns/rows.

```
.container {
  grid-template-columns: 100px 50px 100px;
  grid-template-rows: 80px auto 80px; 
  column-gap: 10px;
  row-gap: 15px;
}
```







