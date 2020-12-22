# Django Rest Framework Permissions

Authentication and Authorization are the two ideas behind allowing some entity access to information.

Authentication is your credentials, proof of who you are.

Authorization is the information providers permission to access information.

- HTTP 403 - Authorized but not Authenticated
- HTTP 401 - Not Authenticated

REST frameworks allows for object-level permissions, where an individual instance of an object has its own access layer for a given user.

Because object level permission can aversely effecty performance, generic views do not apply those object level permissions by default, but can be explicitly called.

The default:

```python
'DEFAULT_PERMISSION_CLASSES': [
    'rest_framework.permissions.AllowAny'
]
```

You may also define permissions per View.

References:

- `AllowAny`
- `IsAuthenticated`
- `IsAdminUser`
- `IsAuthenticatedOrReadOnly`
- `DjangoModelPermissions`
- `DjangoObjectPersmissions`

[<-- Back](../README.md)