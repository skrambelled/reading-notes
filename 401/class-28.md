# Django CRUD and Forms

As you may recall from creating forms in JS, there's a lot of work involved. You have to write the html, the SQL queries, handle the data, validate and sanitize the data. Django does much of that heavy lifting for you.

GET method should be used when data *will not* change through the submission of a form.
POST method should be used when data *will* change.

---

## Django form handling

1. First users asks for the form.
1. Then user submits form.
1. Django validates data, and sends back to the user if form needs updating.
1. Otherise, Django processes the data, and sends user to the proper page.

---

## Django form data fields

Many of the data fields for forms are similar to field you might have seen with models.

- BooleanField
- CharField
- DateField
- There are many form field types, look them up.

Fields can also have specific behaviours defined by their attributes, such as `required`, `validators`, and many more.

---

## Validation

You can override `clean_<fieldname>()` to define your own validation method.

When doing so, make sure you sanitize the incomming data, so as not to have holes in your security.

We can also wrap views with decorator `@login_required` so that users without credentials cannot submit forms.

There is also a cross-site forgery protection token,`csrf_token` that should be included when rendering the form to the user, to reduce attacks from malicious users.

## ModelForms

There is a ModelForm help class, so that you dont have to recreate all the model data into a form, but rather allow Django to manage that for you.

```python
from django.models import ModelForm
```

[<-- Back](../README.md)
