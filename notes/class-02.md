# More on CSS

CSS or Cascading Style Sheets are used to control the appearance of content in HTML

You can manipulate a variety of html elements such as:
- Boxes
- Text
- Tables
- Lists
- Forms

This manipulation is applied by associating rules in CSS to HTML elements. A rule is a selector and a declaration, for e
xample:

```css
p {
    font-family: Arial;
    color: yellow;
}
```

A rule can apply to as many comma separated selectors as you like.

## Link external CSS

Use the `<link>` element inside of the `<head>` to specify where the css file lives.

- Use `<href="filepath">` to point to the filepath.
- Use `<type="text/css">` to declare the type of document, in this case it is CSS.
- Use `<rel="stylesheet">` to specify the relationship of the HTML to the linked document, in this case it is a styleshe
et.

You can `<link>` multiple CSS files into one HTML document

## Internal CSS

You can include CSS internally in an HTML
document by using the `<style>` element, which usually is inside the `<head>` element.

If your site has more than one page, absolutely use an external .css file, rather than using internal CSS.

## Selectors

selector | applies to | syntax
-------- | ---------- | ------
universal | all elements | `* {}`
type | element names | `h1, h1, p {}`
class | all elements with matching class attribute | `.class_value {}`
parent.class | only matching parent elements with matching class attribute | `element_name.class_val {}`
id | match all elements with matching id attribute | `#id_value {}`
Many more, plus also advanced selectors.

## Color

You can specify colors in three different ways.
```css
/* rgb */
h1 {
    color: rgb(100,100,100)
}

/* hsl (hue, saturation, lightness) */
h1 {
    color: hsl(120, 70%, 70%)
}

/* hex */
h1 {
    color: #abc123;
}

/* name */
h1 {
    color: DarkRed;
}
```

Color can be applied in a variety of ways
- background
- foreground
- opacity (when designating opacity, some browsers may not recognize it, so also set a rgb colour for that browser to fa
ll back on)
- hue
- opacity (you can rgba() and hsla(), to assign an alpha value to a 4th parameter)