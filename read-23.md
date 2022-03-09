# Django Best Practices

## Setup

1. Create and navigate into a dedicated directory for code
2. Install Django
3. Make a new Django project
4. Make a new app
5. Start the local web server

- Code:

```
mkdir name && cd name
pipenv install django
pipenv shell
django-admin.py startproject name .
python manage.py startapp name
python manage.py runserver
```

## Create Custom User

1. Update config/settings.py
    1. Add new app to `INSTALLED_APPS`
    2. Add `AUTH_USER_MODEL = 'app.name'`
2. Create a new CustomUser model
    1. Add a class dedicated to the users to the model file
    2. Create a `__str__` method to return name of user on admin site
3. Create new UserCreation and UserChangeForm
    1. Create new python file dedicated to forms
    2. Create a class with a sub class for each form as seen below:

        ```
        from django import forms
        from django.contrib.auth.forms import UserCreationForm, UserChangeForm
        from .models import CustomUser
        class CustomUserChangeForm(UserChangeForm):

            class Meta:
                model = CustomUser
                fields = ('username', 'email')
        ```

4. Update the admin as seen below:

    ```
    from django.contrib import admin
    from django.contrib.auth.admin import UserAdmin
    from .forms import CustomUserCreationForm, CustomUserChangeForm
    from .models import CustomUser

    class CustomUserAdmin(UserAdmin):
        add_form = CustomUserCreationForm
        form = CustomUserChangeForm
        model = CustomUser
        list_display = ['email', 'username',]

    admin.site.register(CustomUser, CustomUserAdmin)
    ```

5. Make and run migrations
    1. `python manage.py makemigrations accounts`
    2. `python manage.py migrate`

## Create a Superuser

- `python manage.py superuser`
- Follow the prompts

### Templates/Views/URLs

1. Add templates to settings (settings.py):

    ```
    TEMPLATES = [
    {
        ...
        'DIRS': [str(BASE_DIR.joinpath('templates'))], # new
        ...
    },
    ]
    ```

2. Set login and logout redirect URLs (settings.py):
    1. `LOGIN_REDIRECT_URL = 'home'`
    2. `LOGOUT_REDIRECT_URL = 'home'`

3. Create Templates
    1. Create a templates folder inside your project folder.
    2. Create a `base.html` and a `home.html` inside that templates folder. You will be adding more depending on your apps needs
    3. Inside your `base.html` use the `HTML5` base format with `{% block content %}` & `{% endblock %}` inside your main
    4. Inside your `home.html` `{% extends 'base.html' %}` acts as your import statement and you will be coding the pages contents inside `{% block content %}` & `{% endblock %}` below the import statement

4. URLs
    1. Create a `urls.py` file inside your app directory
    2. Paste the following code:

        ```
        from django.urls import path
        from .views import SignUpView

        urlpatterns = [
            path('signup/', SignUpView.as_view(), name='signup'),
        ] 
        ```

5. Views
    1. The views.py file will contain the final form:

    ```
    from django.urls import reverse_lazy
    from django.views.generic.edit import CreateView

    from .forms import CustomUserCreationForm

    class SignUpView(CreateView):
        form_class = CustomUserCreationForm
        success_url = reverse_lazy('login')
        template_name = 'registration/signup.html'
    ```

# Useful Links

- [Django Best Practices](https://learndjango.com/tutorials/django-custom-user-model)
- [Django for Professionals](https://github.com/wsvincent/djangox)