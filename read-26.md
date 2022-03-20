# Permissions

- *Permissions*: determine whether a request should be granted or denied access.

## How they are determined

- In REST frameworks they are defined by a list of permission classes
- Before running the main body each permission in the list is checked and if they fail an exception is raised:

    - The request was successfully authenticated, but permission was denied. — An HTTP 403 Forbidden response will be returned.
    - The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers. — An HTTP 403 Forbidden response will be returned.
    - The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers. — An HTTP 401 Unauthorized response, with an appropriate WWW-Authenticate header will be returned.

## Object level permissions

- REST permissions also support object-level permissions. Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.

- I.E.:

```
def get_object(self):
    obj = get_object_or_404(self.get_queryset(), pk=self.kwargs["pk"])
    self.check_object_permissions(self.request, obj)
    return obj
```

## Setting Policy

- This should be set globally for restriction

```

REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}
```

- This will allow anyone access

```
'DEFAULT_PERMISSION_CLASSES': [
   'rest_framework.permissions.AllowAny',
]
```

