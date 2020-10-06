# jQuery

jQuery is a library you can include to select elements and manipulate elements in the DOM using CSS selectors.

`jQuery('p')` would select all `<p>` elements.

`$('p')` is shorthand for the same.

Anything you can do in jQuery can be accomplished in vanilla js, but jQuery is much easier to use in many instances, for example:

* loop through DOM elements
* add or remove DOM elements
* events
* fade elements
* AJAX requests

## Selectors

jQuery can use all of the CSS selector methods you might be familiar with, plus quite a few bonus methods.

Some JQ speciic bonus selectors:

* `:input` - input elements
* `:image` - all images
* `:hidden` - hidden elements
* `:visibile` - visible elements
* `:animated` - elements currently being animated
* many many more, look them up and play with them

## Methods

Once you've selected some objects to mess around with, jQuery offers many methods to get or change content.

* `height()`
* `width()`
* `show()` - reveal hidden elements
* `hide()` - hide elements
* `slideDown()` - animation
* `slideUp()`
* `on()` - event handling
* `stop()` - freeze an animation
* `animate()` - resume an animation
* `append()`, `prepend()`, `before()`, `after()` - instert elements
* `html()` - get or change html content
* `text()` - get or change element text
* `remove()` - remove elements
* `addClass()`, `removeClass()`, `attr()`, `removeAttr()` - class and attribute manipulation
* `css()` - get or change css rules
* `each()` - much like a loop, use `this` or `$(this)` to reference the current element.
* many more!

## References

A jQuery object holds references to DOM elements, rather than copying those elements.

More than one element can be selected through jQuery at once. When applying a method to a set of pointers, jQuery will loop through them automatically, rather than you having to create a manual loop.

## Chaining

jQuery can chain multiple methods together to execute in a sequence.

When chaining methods, each methods should be placed on its own line for readability.

Methods used solely for getting data cannot be chained.

## .ready()

```js
$(document).ready(function() {
  // jQuery script
});
```

The `.ready()` method will fire when the page is loaded, so that you can then operate your script.
However it will not have waited for all the assets to have loaded, for that use `.on()`.

You can also place the script at the just before the closing body tag, to ensure that the HTML (meaning the DOM) is loaded.

[<-- Back](../README.md)
