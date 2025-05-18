2024-08-21

When we connect our queryset keywords with a dot, like *Book.objects.all.filter(xxx).exclude(yyy)*, it's and *AND* statement in SQL. However, if we want to use OR statement, we need the Q() object. Q objects in general let us build more complicated queries


### Hashtags:
#coding #webdev #djangoforprofessionals

### References (source material, similar notes):
https://docs.djangoproject.com/en/5.1/topics/db/queries/#complex-lookups-with-q
https://docs.djangoproject.com/en/5.1/ref/models/querysets/#query-related-tools
[[Search functionality with Django - needs more in-depth]]