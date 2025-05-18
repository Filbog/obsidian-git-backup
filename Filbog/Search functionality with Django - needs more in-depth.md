2024-08-21


For this, we can use the **querysets**. Example of a simple search with a search form and querysets on the backend: https://github.com/Filbog/django-for-pros-ch7

Advanced search possibilities via *Django for Professionals*:

There are several third-party packages with enhanced features such as **django-watson** or **django-haystack** however, given that we’re using PostgreSQL as the database, we can take advantage of its **full text search** and other features which are built into Django itself.

A final option is either use an enterprise-level solution like **ElasticSearch** that must be running on a separate server (not the hardest thing with Docker), or rely on a hosted solution like Swiftype or Algolia.

### Hashtags:
#django #webdev #djangoquerysets #djangoforprofessionals

### References (source material, similar notes):
https://github.com/etianen/django-watson
https://github.com/django-haystack/django-haystack
https://docs.djangoproject.com/en/4.0/ref/contrib/postgres/search/
https://www.elastic.co/
[[Complex queries with Q() objects in Django]]