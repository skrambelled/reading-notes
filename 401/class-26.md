# Django

Django is a web app framework for Python. You can install it using pip:

```bash
$ python -m pip install Django
```

Once you have Django installed you can start a new project:

```bash
$ django-admin startproject <project>
```

This will set up a few files for you, so that you can get started with Django.

```bash
project/
    manage.py
    project/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
```

Then you can issue the following command:

```bash
$ python manage.py runserver
```

Django comes with a webserver meant for development, but is not intended for production environments, so get Apache or some production level web server when you are deploying your web app.

You can optionally define a port by adding it as an argument in the above `runserver` command, otherwise it will default to port 8000. This webserver will reload itself as you modify files, like you maye have experienced with nodemon when useing NodeJS.

Now in your urls.py file you can define enddpoints, which are called url patterns in Django.

```python
urlpatterns = [
    path('blah', include('blah.urls')),
    path('admin', admin.site.urls)
]
```

Always use `include()`, except with `admin.site.urls`. Include allows for relative paths by chopping off the preeamble to the matched string, and then passing the remaining bits to your webserver.

`path()`takes 4 arguments, 2 of which are required and the other 2 are optional.
route and view are required, while kwargs and name are optional.

[<-- Back](../README.md)
