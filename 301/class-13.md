# Sending Form Data

HTML forms have a variety of elements for the user to interact with, and a variety of ways for you to validate their data. We'll focus on sending the data though.

the `action` attribute of a `<form>` defines where the data gets sent to upon submission.

```html
<!-- A form's data can be sent to a URL -->
<form action="http://somewhere.com/someform">

<!-- Or locally, using relative filepaths -->
<form action="page/in/my/site">

<!-- Or if no action is defined, to the same page where the form resides -->
<form>
```

## From the client

If you send a form using http (not encrypted) from a secure site, the user will be warned.

You can also send a form over https (encrypted) from a non-secure site.

the `method` attribute determines which POST method to use

```js
// GET will result in a form url like http://somwhere.com?input_field=input_value
<form method="GET">

// POST will append the form data to the HTTP body
<form method="POST">
```

## On the server

Depending on your server and also the expected data, you will need some way to handle the routes (endpoint and method).

For examples, on node.js (without any sort of actual SQL or error handling)

```js
app.post('/this', (req, res) => {
  // handle the req data here, from the http
  client.request(SQL_QUERY, values);
  
  // tell the user they did it
  res.send('success!');
});
```

## Security

Never ever trust incomming data. It must be 'sanitized', meaning escape all special characters, limit the ammount of data, and quarantine file uploads.

[<-- Back](../README.md)
