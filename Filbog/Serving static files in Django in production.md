
### WhiteNoise

In local development, Django's built-in server (used with *runserver*) performs many functions, including serving static files. But for production env, this does not work - really inefficient or sth. We need a package like [WhiteNoise](https://whitenoise.readthedocs.io/en/stable/):
"With a couple of lines of config WhiteNoise allows your web app to serve its own static files, making it a self-contained unit that can be deployed anywhere without relying on nginx, Amazon S3 or any other external service. (Especially useful on Heroku, OpenShift and other PaaS providers.)"
Works really well with Django

### collectstatic
As said before, the local server serves the files for us but it's inefficient in prod since it has to perform request for each resource. Instead, it's better to have all files in one location and serve them as a large HTTP request. For this we have the command ***[collectstatic](https://docs.djangoproject.com/en/5.1/ref/contrib/staticfiles/#collectstatic)***




#django #coding #webdev