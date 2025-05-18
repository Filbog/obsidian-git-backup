[Django docs](https://docs.djangoproject.com/en/4.2/ref/urlresolvers/#reverse-lazy)
Bottom line: we use it when working with generic class-based views, especially with DeleteView, when providing url to *success_url*. Or with redirecting upon form submission, like in sign up class-based views.
