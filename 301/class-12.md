# EJS partials

When you want to recycle a smaller bit of a page amongst several pages, you can use EJS partials.

For example, you might have a `<header>` and `<footer>` partial,
rather then rewriting that code in several places.

Here is a navbar example, take note that we use the <%- %> syntax, so that the HTML is not escaped.

```html
<!-- partials/navbar.ejs -->
<nav>
  <ul>
    <li><a href="somplace.com">someplace</a></li>
    <li><a href="anotherlink.org">another</a></li>
  </ul>
</nav>
```

```html
<!DOCTYPE html>
<html>
<head>
  <title>navbar example of an ejs partial</title>
</head>
<body>
  <%- include('partials/navbar') %>
  <div>Content here</div>
</body>
</html>
```

[<-- Back](../README.md)