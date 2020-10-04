# CSS Layout

## Attractive page layouts

block-level vs inline

In the Box model block-level elements are on their own new line, whereas inline elements are displayed side-by-side on the same line.

It is common to group elements within a block-level container.

This nesting can go as deep as necesary.

### Positioning:

- normal flow - an elements position is unchanged according to the flow
- relative - an element's position is relative to its normal position
- absolute - an element's position is relative to its container
- fixed - an element's position is fixed relative to the DOM's window
- float - an element floats in a position relative to its sibling content
- z-index - gives a z-axis depth to elements

```css
  p.stuff {
    position: relative;
    top: 20px; /* move the stuff class down 20px, because we are adding more top+ */
    left: 10px; /* move the stuff class right by 10px, because we are adding more left */
  }
```

### fixed-width

pros | cons
---- | ----
accuracy in dimensions | can have gaps on the edges
greater control over flow | higher resolution screen can render small text
line length is controllable | varying font sizes may not fit
image is of static size | resolution is not dynamic

### liqiud layout

Liquuid layouts depend on the users window size, and will shape around that size.
This means you have less control over the layout, but allows for a more interactive space.

### 960-gs

960-gs is a paticular layout structure which you can explore!

### @import

You can import stylesheets into one another using @import, this is how css handles inheritance!!!

[<-- Back](../README.md)
