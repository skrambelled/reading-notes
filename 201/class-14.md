# CSS Transforms and Transitions

## Transforms

2d transforms in css:

- `transform: rotate('deg')` - rotate cw 20 deg, you can use negative values for ccw
- `transform: scale(num)` - make element appear larger. use fractional values less than 1 to get smaller
- `transform: scaleX(num)` - to only scale the X axis, or `scaleY()` to scale the Y axis
- `transform: translate(x,y)` - move and image by x and y pixels.
- `transform: translateX(num)` - mvoe an image on the x axis, `translateY()` for Y axis
- `transform: skew()` - to skew an image by degs
- You can combine these transforms.

3d
For 3d transforms to work, they need a perspective to operate around.
Consider the perspective as if it were a vanishing point somewhere in space.

Perspective can be set two ways:

- within the transform property on individual elements
- on the transform property of the parent element

transforms in 3d:

- Can `rotate` around Z axis in 3d space
- Can `scale` in the Z axis
- Can `translate` in the Z axis
- Cannot `skew` it the Z axis
- `backface-visibility : [hidden / visible]`

## Transitions

CSS can perform transitions natively without Flash or JavaScript

`transition-property` will declare which properties a transition is applied to, and supports a comma separates list of properties when you want to apply a transition to more than one at a time.

Not all properties can be transitioned, so look them up when using this.

`transition-duration` will specify how much time the transition should take place over.

`transition-timing` will specify the transition curve, such as the property `ease-out`. There are several preset curves but you can specify your own with `cubic-bezier` and `steps`.

`transition-delay` can stall the transition's start time.

`@keyfrmes` can target sections of animation.

You can apply transitions very easily, for example:

```css
.fade {
  opacity: 0.5;
}

.fade:hover {
  opacity: 1;
}
```

## Animations

There are unlimited techniques, here [here are some good examples](http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users).

[<-- Back](../README.md)
