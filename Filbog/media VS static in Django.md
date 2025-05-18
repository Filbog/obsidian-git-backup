2024-08-20

static assets that developers configure are, you guessed it, **static**. User-uploaded files are referred to as **media**. With static files, we can trust them for the most part. It's totally different with media though and we **ALWAYS** have to validate them.
We should also store them on a dedicated CDN (Content Delivery Network), not on our own server. Django has a package for it - django-storages.


### Hashtags:
#django #webdev #djangoforprofessionals

### References (source material, similar notes):
https://docs.djangoproject.com/en/5.1/ref/models/fields/#file-upload-security
https://docs.djangoproject.com/en/5.1/topics/security/#user-uploaded-content-security
Django for Professionals - has a walkthrough on enabling basic file upload