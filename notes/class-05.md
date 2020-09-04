# Images, Color, Text

## Images

A picture is worth 1000 words, as they say. Images are able to convey a message or set the tone of a page or site.

Organize your images into a sensible file structure hierarchy for your site.

```html
<img src="URL or filepath" alt="text description">
<!-- title="mouse hover text" is an optional image attribute -->
```

`height` and `width` are common attributes, and `align` is old, use CSS instead to manage the flow of other content around an image.

- jpg - use for images with many colors
- gif or png - for images with fewer color are large areas of little color
- bmp - for vector iamges
- gif - for animated images

You should save an image by the same height and width as it will appear on the page and at 72ppi for optimization and also to avoid distortion.

To caption an image:

```html
`<figure> <img src = "..." alt = "..."> <figcaption>Some caption</figcaption> </figure>
```

## Color

### Many formats

- color name
- Hex
- `rgb()` or *`rgba()` for opacity*
- `hsl()` or *`hsla()` for opacity*

### Contrast

High contrast leads to better legibility, though slightly lesser contrast on large ammounts of text will strain the eyes less.

If text is light on a dark background, increasing the space between lines can make it easier to read.

[A handy tool.](https://snook.ca/technical/colour_contrast/colour.html#fg=33FF33,bg=333333)

## Text

Two general categories of text properties:

1. affect the font directly,  like:
   - typeface
   - bold
   - italics
   - size

2. affect the text regardless of font, like:
   - color
   - spacing

### Font

Some groups of fonts:

- Serif
  - extra details at the ends of letters
- Sans-serif
  - straight ends to letters
- Monospace
  - fixed width
- Cursive
  - elements of handwriting
  - joining strokes
- Fantasy
  - decorative, used for titles, but not long blocks of text

Dont use more than 3 fonts on a page.

#### Attributes

- `font-family`
- `font-size`
- `font-style`
  - "normal", "italic", "oblique"
- `font-weight`
  - "normal", "bold"
- `text-transform`
  - "uppercase", "lowercase", "capitalize"
- `text-decoration`
  - "none", "underline", "overline", "line-through", "blink"
- `line-height`
- `letter-spacing`
- `text-align`
- `vertical-align`
- `text-indent`
- `text-shadow`

```css
p:first-letter {
  /* attributes for first letter of text */
}

p:first-line {
   /* attributes for first line of text  */
}

a:link {
  /* attributes for not visited links */
}

a:visited {
  /* attributes for visited links */
}

:hover {
  /* attributes for hover over elements */
}

:active {
  /* attributes for active elements (like being clicked on) */
}

:focus {
  /* attributes for elements that have current browser focus */
}
```

[<-- Back](../README.md)