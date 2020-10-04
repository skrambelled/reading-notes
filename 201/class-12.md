# charts.js

Charts.js is an open license API for making awesome charts and graphs.

## `<canvas>`

The `<canvaas>` element can look initially similar to the `<img>` element, but without a `src` or `alt` attribute.

A canvas is by default, 300px wide by 150px tall, but can be resized by the DOM or CSS.

Use an id element to uniquely target a canvas, like any other element.

`<canvas>` requires a matching `</canvas>` tag.

### Fallback content

Define fallback content for when the browser or user setup does not support a canvas.

`getContext()` can allow JS to determine if fallback content is needed.

### `draw()`

Is called after the page loads by listening for the `load` event on the document object.

The coordinate space starts at 0,0 in the top left by default. Other spaces are available.

#### examples

```js
function draw() {
 var canvas = document.getElementById("canvas");
 if(canvas.getContext()) {
   // we support canvas and can do operations
   var ctx = canvas.getContext('2d');

   // fill a rectangle
   ctx.fillRect(50,50,200,200);
 } else {
   // we do not support canvas and have to use fallback operations
 }
}
```

Draw can draw rectangles, or it can draw shapes defined by point.

Canvas is ultimately a very robust API, and needs extensive practice to master.

[canvas tutorials](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial)

[<-- Back](../README.md)
