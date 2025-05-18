28-10-2024

In general - Django 5.1 comes with that usable_password property, so if we use custom user model, we have to overwrite it. If not, then we get error in Django Admin when creating a new user. The dude on Stackoverflow says to do it in the forms. I, on the other hand, did this in admin in add_fieldsets (aerial-calendar repo)
### Hashtags:


### References (source material, similar notes):
https://github.com/Filbog/aerial-calendar
https://stackoverflow.com/questions/78850636/what-is-password-based-authentication-in-the-usercreationform-in-django-and-how