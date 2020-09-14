# Images and Practical Information

## Images

### Centering

- first images are inline by default so you can use CSS to declare an img as a block level element `display: block;`
- then you can use `text-align: center;` on the parent or you can use `margin: auto;` on the img itself.

### Background

```css
body {
  background-image: url("assets/bg-image");
  background-repeat: repeat;
  /* repeat-x; or repeat-y; to repeat in one direction */
  /* no-repeat; to not repeat at all */

  /* alternatively you can use */
  background-attachment: fixed;
  /* to keep the image fixed on the page. or  */
  background-attachment: scroll;
  /* to have it scroll */

  /* or even */
  background-position: right bottom; /* etc */
}
```

`background:` shorthand arguments ordering is as follows:

1. `background-colour`
2. `background-image`
3. `background-repeat`
4. `background-attachment`
5. `background-position`

You can use sprites (using one different areas of one image) to assign differint images to states of HTML objects. such as a hover state, or an active state.

### Video

HTML5 supports a native video (and audio) player experience, though each browser will have implemented this in its own way.

You can use CSS and JS to modify the player quite significantly.

[A good resource about video and audio in the browser.](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs)

## Practical Information

### SEO (Search Engine Optimization)

#### On page techniques

- Seven key places:
  1. page title
  1. url
  1. headings
  1. text
  1. link text
  1. image alt text
  1. `<meta>` tag in the head

Research keywords.

#### Off page techniques

Get sites to link to you.

Words that appear between the `<a>` tags matter. If they are relevant rether than just "Click here", that has a positive influence. This is true for your outgoing links and also incomming links from external pages.

### Google Analytics

Can give you insight into how you might improve your site through a variety of metrics:

- enter / exit info
- activity info
- bounce info
- search terms to reach your site
- lots more!

[<-- Back](../README.md)
