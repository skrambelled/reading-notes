# RWD (Responsive Web Design)

## Flexible layouts

Flexible layouts allow a web page to respond dynamically to varying viewport sizes. They are built using relative units, like `em` units or percentages so define positioning and sizes of elements.

Ethan's simple formula for deciding percentages:

`target ÷ context = result`

This approach allows you to have content dynamically sized according to some percentage of the containing element (and eventually the viewport), but this breaks when you get too small or too large of a viewport, which is
when you need to use media queries.

## Media queries

As more and more internet connected devices are able to access web pages, we need to be more aware of their screen size or interactive methods like a mouse or a touch screen.

You can use media queries in CSS3 to target devices with particular attributes, such as:

```html
<link rel="stylesheet" type="text/css"
  media="screen and (max-device-width: 480px)"
  href="smallscreen.css" />
```

You can also insert media queries directly into CSS using `@media` (or `@import`):

```css
@media screen and (max-device-width: 480px) {
  p {
    font-size: 12px;
  }
}
```

Media query types:

* `all`
* `screen`
* `print`
* `tv`
* `braille`
* More types are supported over time

Media query operators:

* `and`
* `not`
* `only`

Media query features:

* `height`
* `width`
* `spect-ratio`
* `pixel-ratio`
* `resolution`
* `orientation`
* can use `min` and `max` prefixes with several features, like `min-height`


[<= Back](README.md)
