2024-08-17

Via Django for pros, chapter 11:
"It can be confusing whether to use a primary key (PK) or an ID in a project, especially since Django’s DetailView treats them interchangeably. However there is a subtle difference.

The id is a model field automatically set by Django internally to auto-increment. So the first book has an id of 1, the second entry of 2, and so on. This is also, by default, treated as the primary key pk of a model.

However it’s possible to manually change what the primary key is for a model. It doesn’t have to be id, but could be something like object_id depending on the use case. Additionally Python has a built-in id()151 object which can sometimes cause confusion and/or bugs.

By contrast the primary key pk refers to the primary key field of a model so you’re safer using pk when in doubt."
So ID is created by default for new instances of an object. ID is what's usually set as a primary key, but it doesn't have to be ID - it can be any property of a model for that matter.
### Hashtags:
#coding #django #webdev #djangoforprofessionals

### References (source material, similar notes):
