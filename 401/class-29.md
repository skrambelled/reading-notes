# Django Custom User Model

Django has a built in User model for authentication, however you should use a custom user model for real implementations.

When you build your custom user model, extend it from AbstractUser, which itself extends from AbstractBaseUser.

We can then make a create user and update user form, on the appropriate templates.

See this [tutorial](https://learndjango.com/tutorials/django-custom-user-model) for creating a customer user model.

A massive advantage of this method is that you can add additional fields to your model whenever you like!

The keys steps from this [video walkthrough](https://www.youtube.com/watch?v=eCeRC7E8Z7Y):

1. make an user or account app and add it to INSTALLED_APPS in settings.py
1. make a user or account model within this account map
   1. extending from `AbstractUser`
   1. decide how a user logs in, email vs username
   1. add required fields to your model: `email`, `username`, `date_joined`, `last_login`, `is_admin`, `is_active`, `is_staff`, `is_superuser`
   1. you can add additional fields, like first_name, favorite_color, etc... but those ones above are required
   1. `USERNAME_FIELD` needs to be set, this is the field that users will use to login, such as 'email'
   1. `REQUIRED_FIELDS` also needs to be set, for a list of required fields
   1. some required functions for the model:
      - `has_perm()`
      - `has_module_permissions()`
   1. associate the model with a custom user manager
1. make a custom user manager
   1. this also has required methods:
      - `create_user()` - this methods needs to raise ValueErrors when not supplied with required fields, like email or username.
      - `create_superuser()` - similar to create_user, but used for making admin accounts
1. To override django's default user model, assign your custom model to `AUTH_USER_MODEL`
in `settings.py`
1. And of course, register the new model and `makemigrations` and `migrate`...

[<-- Back](../README.md)
