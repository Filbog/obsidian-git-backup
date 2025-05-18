2024-08-17

It's a method to set the URL to specific instances of the model in one place (within the model), instead of hard-coding the url in every place in HTML separately - then, if we change the URL, we'd have to change the hard-coded URL in every place. Instead, with get_absolute_url method we just set the url in one place, and then in HTML we just use this method. This is a cleaner approach and should be used whenever you need individual pages for an object.


### Hashtags:
#django #coding #webdev #djangoforprofessionals

### References (source material, similar notes):
Django docs: https://docs.djangoproject.com/en/5.1/ref/models/instances/#django.db.models.Model.get_absolute_url 
Repo where it's used: https://github.com/Filbog/django-for-pros-ch7