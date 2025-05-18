[[Django Deployment Checklist]]

 
 Before even touching fly.io:
- [ ] add **.dockerignore** file in root dir
	- add stuff like venv/ folder, __pychache__/, database (if using SQLite), .git
- [ ] once we know the urls for our website, add those to ALLOWED_HOSTS and CSRF_TRUSTED_ORIGINS

On fly.io:
 - *fly auth login* - log in to fly.io
 - *fly launch* - for creating the Dockerimage of our website that'll later be deployed and setting up stuff in general for the deployment
 - *flyctl* *deploy* - to actually deploy our website
	 - As for today (05/05/2024) I don't know why but Dockerfile has different ports than those needed to be listened for on fly.io... So I have to manually change EXPOSE 8000 to 8080 and the gunicorn command from 8000 to 8080 for the app to work on fly.io
 - *fly apps open* - to open the website url
 - *fly ssh console --pty -C "python /code/manage.py createsuperuser"* - this is to create admin

#django #coding #webdev #flydotio #deployment