# Authentication & Production Server

## What is JSON Web Token

- JSON Web Token is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object

## When to use JWT

1. *Authorization*: Most common. Each time there is a request it will include a JWT allowing access
2. *Information Exchange*: JWT provide private keys that allow for verification of identity keeping the information secure

## Structure

- *Header*: Two parts type of tokens and signing algorithm:

```
{
  "alg": "HS256",
  "typ": "JWT"
}
```

- *Payload*: This contains there claims. The registered, public, and private claims:

```
{
  "sub": "1234567890",
  "name": "John Doe",
  "admin": true
}
```

- *Signature*: Used to verify message wasn't changed during transfer:

```
HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)
```

# JWT Authentication with Django REST Framework

## Installation

- `pip install djangorestframework_simplejwt`

- Settings.py:

```
REST_FRAMEWORK = {
    'DEFAULT_AUTHENTICATION_CLASSES': [
        'rest_framework_simplejwt.authentication.JWTAuthentication',
    ],
}
```

- urls.py:

```
from django.urls import path
from rest_framework_simplejwt import views as jwt_views

urlpatterns = [
    # Your URLs...
    path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
    path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
]
```

# Useful Links

- [How to Use JWT Authentication with Django REST Framework](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)
- [Django Runserver Is Not Your Production Server](https://vsupalov.com/django-runserver-in-production/)
- [Introduction to JSON Web Tokens](https://jwt.io/introduction/)