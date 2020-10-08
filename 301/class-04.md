# CSS grids

## Grid containers

[Grid practice game](https://cssgridgarden.com/)

```css
.container{
  display: grid | inline-grid;
}
```

A grid allows you to define rows and columns in css.

* `grid-template-rows: val1 val2 val3 ... ;`
* `grid-template-columns: val1 ... ;`

Values can be `%`, `em`, `px`, or even `fr` (fractions)

You can use `repeat(num, val)` to create more than val.

`grid_area` will combine `grid-template-rows` / `grid-template-columns`

Grid gaps can set 'gutters' between the cols or rows.

* `column-gap`
* `row-gap`
* `grid-column-gap`
* `grid-row-gap`
* `gap: <row-gap> <col-gap>` shorthand

Like in flexbox, you can justify, but use `justify-items` to move children elements along the main axis (row axis).

Similarly, `align-items` will handle the cross axis (col axis).

`place-items` is shorthand for both.

And `justify-content` and `align-content` will adjust the internal content as a when your content is smaller than your grid.

`place-content` is a shortcut for both.

`grid-auto-flow` can adjust the configuration of how grid items are handled when they are places outside of the grid, see documentation for details.

## Grid children

Define how much space within a grid an element takes up. Starts at 1.

* `grid-column-start: val;`
* `grid-column-end: val;`
* `grid-row-start: val;`
* `grid-row-end: val;`
* `grid-column: start / end;` - shorthand
* `grid-row: start / end;` - shorthand
* `grid-area: row-start / col-start / row-end / col-end;` - shorthand for all

`justify-self` to modify the row-axis alignment of this child within its grid space.

`align-self` to modify the col-axis alignment of this child within its grid space.

`place-self` is shorthand for both.

[<-- Back](../README.md)
