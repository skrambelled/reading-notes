# Flexbox

Flexbox is implemented through a relationship of properties of a parent and their children, but keep in mind, parents can also be children to their own parents.

[flexbox guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## Properties for the parents

```css
.container {
  display: flex;
}
```

This will define all container class elements as flexbox containers, so that their direct children will be able to use flexbox properties and that the parent themselves can define the flow of their flexbox system.

* `flex-direction: row (default) | row-reverse | column | column-reverse;`
* `flex-wrap: nowrap (default) | wrap | wrap-reverse;`
* `flex-flow: (flex-direction) (flex-wrap);`
* `justify-content: flex-start (default) | flex-end | center | space-between | space-around | space-evenly;`
* `align-items: stretch (default) | flex-start | flex-end | center | baseline | much more, see link below`
* `align-content: flex-start | flex-end | center | stretch | space-between | space-around`


## Properties for the children

* `order: num;` - changes the ordering of that element, by val which can by positive or negative values. 0 is default.
* `flex-grow: num;` - a proportion of how much room an element can occupy compared to its original size. 2 would be twice as large, but this is in relation to all of its siblings as well.
* `flex-shrink: num;`
* `flex-basis: val | auto ( default);` - set the fault size of an element.
* `flex: (flex-grow) (flex-shrink[optional]) (flex-basis[optional])` - shorthand
* `align-self: auto (default) | flex-start | flex-end | center | baseline | stretch;` - allows an item to individually place itself.

[<-- Back](../README.md)
