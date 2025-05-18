
It's used to **add information to a template by updating the context, a dictionary object containing all the variable names and values available in our template**

For performance reasons, Django templates compile only once; if we want something available in the template, it must load into the context at the beginning. So sometimes want to override/extend get_context_data() to add stuff to the "context".

Django docs:
[get_context_data()](https://docs.djangoproject.com/en/4.2/ref/class-based-views/mixins-simple/#django.views.generic.base.ContextMixin.get_context_data)
[context](https://docs.djangoproject.com/en/4.2/ref/templates/api/#django.template.Context)

Cool example of it in action is in Django for Beginners, Newspaper Project, Adding Comments section. In my code it's in newspaper_project/articles/views.py