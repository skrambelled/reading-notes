# Structure web pages using HTML

## Who is the site for?

Is this site for individuals? What demographics are you targetting?

* age
* gender mix
* income
* education
* site usage
* devices used to access the site

Is this site for companies?

* What purpose does it serve?
* Are people visiting this site on behalf of others?
* What is the visitors position within their company?
* What sort of budget allocation do you expect them to have?

Invent fictional characters to help tell the story of why they may
be visiting your site:

Name | Alfred | Betty | Clayton
---- | ------ | ----- | -------
Gender | Male | Female | Male
Age | 52 | 65 | 35
Location | Gotham | New York | L.A.
Occupation | Butler | Cartoonist | Tennis Player

## Create a site map

Orangize information into a hierarchical structure, that makes sense
from the consumer's point of view.

* Group similar information into subcategories
* Create concise, clear and selective navigation, sometimes even as a subset of a selection of information, if needed.

## Wireframes

Sketch out the design of the site, or pages within the site to guide your design decisions.

## Using design to communicate

Make important parts of the site or page distinct to draw attention, or less  distinct to do the opposite.

Group similar information into chunks or blocks for user simplicity.

Use contrast in _**style**_, `<span style="color:red">color</span>` or `<span style="font-size:2em">size</span>` to communicate key messages.

Use spacing to group similar items together.

## Navigation

Navigation should be clear, concise, and selective.

Navigation should be grouped appropriately, sometimes with secondary or even tertiary navigation.

Navigation should give the user context, be interactive and consistent.

## Web page structure within HTML5

Historically, the `<div>` element has been used to structure web pages, but with HTML5 several new elements have been introduced. These new elements have explicit uses, and when putting content into a page outside the scope of these conditions you should still use the `<div>` element.

Some examples of new elements:

```html
<header>
<nav>
<article>
<section>
<aside>
<figure>
<footer>
```

To ensure that older browsers can view content even though they may not support HTML5, you need to check the browser versrion.

## Extra Markup

### Deprecation

Over time HTML versions have been released, and browsers updated or created to support newer versions.
Some elements of HTML are introduced with each new version, while others are removed.

You should avoid elements that CSS can address more efficiently, such as:

```html
<center>
<font>
<strike>
```

### XHTML and XML

HTML4 and XML concepts were combined to create XHTML, which has stricter rules than HTML had beforehand.

* All elements must have a closing tag, except empty elements
* Sub-elements must be closes within their parent element
* Attributes must be in lowercase
* Attributes must be enclosed in double-qoutes
* Deprecated elements should no longer be used

### DOCTYPE

Use the `<!DOCTYPE html>` tag to express to the browser which html version you are using.

### Comments

* HTML uses `<!-- comment -->` syntax.
* Comment your code appropriately. You may not recall its purpose sometime down the road.
* Anyone may view the source code and reveal these comments.
<!-- Here's a fun hidden comment for those of you who view the source code of this page! -->

## id and class attributes

Every element can be assigned an id attribute which can then be used to uniquely identify it within CSS.

Similarly, every element may also carry a class attribute. Unlike id, class may be used to identify groups of elements who need to share CSS rules.

## Block level elements and inline elements

Some elements will force a new line. Some examples:

```html
<h1>
<p>
<ul>
<li>
```

Other elements may be places inline, such as:

```html
<a>
<b>
<em>
<img>
```

`<div>` acts as a container for other elements, or when content has no specific element and will imply a newline.
`<span>` acts like `<div>`, but does not imply a newline as seen here.

`<iframe>`
<iframe
  src="iframe.md">
</iframe>

## Meta data

Meta data is contained within the `<meta>` element contained within the `<head>` element, and is used to describe information about the page that is not visible to the user, for example: timestamping the page, including search engine support or cache instructions.

## Escape characters

HTML uses specific characters like "&lt;" and "&gt;" to denote code. If you'd like to display those characters you need to use a special escape sequence.

Additionally, HTML may also display special characters like &copy; which also require special escape sequences.

Some fonts may not support these special symbols, so double check!

[<= Back](README.md)
