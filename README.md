# Django Example: Book List

This example demonstrates the basic usage of Django, including creating a model, views, URL routes, and a template. Suppose you have an application to display a list of books.

## Create a Model:

```python
# myapp/models.py
from django.db import models

class Book(models.Model):
    title = models.CharField(max_length=100)
    author = models.CharField(max_length=50)

    def __str__(self):
        return self.title
