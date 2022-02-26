# Intro to Django

## What is Django?

- Django is a open sourced Python-based web framework

- First and foremost you need to install *Django*:
  - `python -m pip install Django`

## Object-relational mapper

- This is written as a python class:
  - `class Food(models.Model):`

## URLs and views

- `from django.urls import path`
`from . import views`
`urlpatterns = [path('bands/, views.band_listing, name='band-list')]`

- Import:
`from django.shortcuts import render`
`def band_listing(request):`
  `bands = models.Band.``objects.all()`
  `return render(request, 'bands/band_listing.html',``{'bands':bands})`

- Templates:
  - This is done in `<html>`
  - `{% for x in x %}`: can generate the html element for each x in x

- Forms:
  - `from django import forms`
  - `class Form(forms.Form):`

- Authentication:
  - `from django.contrib.auth.decorators import`
  `login_required`
  `from django.shortcuts import render`
  `@login_required`
  `def my_protected_view(request):`
  `return render(request,'protected.html','current_user:request.url)`

- Admin
  - `from django.contrib import admin`
  - `class MemberAdmin(admin.ModelAdmin):`
  - `admin.site.register(name)`

- Internationalization
  - Django offers full support for translating text into different languages, formatted dates, times, numbers, and time zones.

# Useful Links

- [Why Django?](https://www.djangoproject.com/start/overview/)
- [How Django Works Behind the Scenes](https://wsvincent.com/how-django-works-behind-the-scenes/)