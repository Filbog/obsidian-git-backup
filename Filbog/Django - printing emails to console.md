2024-08-11

Useful when we're building the project and want to set up email registration etc, but don't have SMTP server yet. We have to add this line to *settings.py*:
```python

EMAIL_BACKEND = "django.core.mail.backends.console.EmailBackend"
```


### Hashtags:

#coding #webdev #django #djangoforprofessionals
### References (source material, similar notes):
