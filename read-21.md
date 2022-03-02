# Django Models

- *Models*: Define the structure of stored data,including the field types and anything else pertaining to the format.

## Designing Models

- Before coding it is important to understand what data we need to store and its relationship to one another
- *Django* allows you to define the relationships between data as `(OneToOneField)`, one to many `(ForeignKey)` and `(ManyToManyField)`

## Code Setup Example

```
from django.db import models

class MyModelName(models.Model):
    """A typical class defining a model, derived from the Model class."""

    # Fields
    my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')
    ...

    # Metadata
    class Meta:
        ordering = ['-my_field_name']

    # Methods
    def get_absolute_url(self):
        """Returns the url to access a particular instance of MyModelName."""
        return reverse('model-detail-view', args=[str(self.id)])

    def __str__(self):
        """String for representing the MyModelName object (in Admin site etc.)."""
        return self.my_field_name
```

## Creating or Modifying Data

- This can be done by modifying the data when calling it:
    ``` record.field_name = "New Data"
        record.save()
    ```

## Accessing Data

- This can be done simply using built in python functions:
  - `.all()`
  - `.filter()`
  - `.count()`

## Registering Models

- Import the Models to the python file then type `admin.site.register(Model)`

## Create A Superuser

- This user will have full admin power to the website:
    `python manage.py createsuperuser`

# Useful Links

- [Using Models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models#summary)
- [Django Admin Site](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)