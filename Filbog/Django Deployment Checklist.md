From "Django for Beginners":
*Django defaults to a local development configuration with the startproject command, which makes it easier to start building apps locally, but many settings are a security risk in production.

*Since deployment requires many discrete steps, it is common to have a “checklist” for these since there quickly become too many to remember.*

For details on most of those either look up specific stuff or just go to Deployment section for the later projects in Django for Beginners

Deployment checklist:
- [ ] Install **Gunicorn** as a WSGI server: ***python -m pip install gunicorn==<curr_version>***
	 - The *-m* flag tells Python to run the *PIP* module as a script which ensures that we use the correct version of *PIP* for the Python interpreter we're running - useful if we have multiple *PIP* modules installed, so there will be no conflicts with versions etc.
- [ ] Install **PostgreSQL** (w/brew) - ***brew install postgres*** - only once
- [ ] Install **psycopg** to connect to the PostgreSQL db
	-  "psycopg[binary]"
- [ ] Install **environs** for environmental variables
	- "environs[django]" 
- [ ] update **DATABASES** in settings.py so that it's PostgreSQL in prod, SQLite locally
- [ ] install **WhiteNoise** for static files
	- We also have to update some settings in settings.py
	- remember to run *python manage.py collectstatic*
- [ ] generate **requirements.txt** - ***python -m pip freeze > requirements.txt***
- [ ] Create .dockerignore file
- [ ] Create a .env file
- [ ] Update .gitignore
- [ ] update **ALLOWED_HOSTS** and **CSRF_TRUSTED_ORIGINS** in settings.py 
	- ALLOWED_HOSTS should only have access to local port and actual prod URL
	- CSRF_TURSTED_ORIGINS should only have access to actual prod URL
- [ ] Update **DEBUG** and **[[Generating secret key in django|SECRET_KEY]]|** with environmental variables and values in .env file


#coding #django #webdev #deployment #checklist

References (source material, similar notes):
[[Making our Django app bulletproof and secure - security measures in production]]