2024-08-17

### The problem with id
"Using the pk field in the URL of our DetailView is quick and easy, but not ideal for a real-world project. The pk is currently the same as our auto-incrementing id. Among other concerns, it tells a potential hacker exactly how many records you have in your database; it tells them exactly what the id is which can be used in a potential attack; and there can be synchronization issues if you have multiple front-ends." - so okay for small projects, but can be a security concern and potential synchronization problems if the project grows biiig.

### So what to use instead of id? Slugs vs UUIDs
**"slug"** - a short string representing the object, like in case of Django for Professionals book it'd be *django-for-professionals*. There exists a SlugField model field in Django even. Although, apparently it also can cause synchronization issues when the project grows big. We also have to be able to handle duplicates, like by adding random numbers to the end of the string or sth.
According to *Django for Professionals* author, the best approach is UUID - Universally Unique IDentifier. It's a random string of characters that guarantees uniqueness in any practical scenario. It also has its own model field - UUIDField.

So best to use UUIDs in general
### Hashtags:
#coding #djangoforprofessionals #webdev #security

### References (source material, similar notes):
[[Django - Primary Keys vs IDs]]
[UUIDs in Python's Official Docs](https://docs.python.org/3/library/uuid.html#module-uuid)
[UUIDField](https://docs.djangoproject.com/en/4.0/ref/models/fields/#django.db.models.UUIDField)
[UUID on Wikipedia](https://en.wikipedia.org/wiki/Universally_unique_identifier)
