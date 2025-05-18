2024-08-09

Example - this can be in project-level urls.py:
```python 
from django.contrib import admin
from django.urls import path
from django.http import HttpResponse

urlpatterns = [
    path("admin/", admin.site.urls),
    path(
        "",
        lambda request: HttpResponse(
            "Hello in my bookstore, world! Now with PostgreSQL db"
        ),
    ),
]
```
So basically using anonymous/lambda function to not have to create a separate view in views.py, and/or a template. Can be useful for quick debugging or sth.
### Hashtags:
#django #coding

### References (source material, similar notes):
