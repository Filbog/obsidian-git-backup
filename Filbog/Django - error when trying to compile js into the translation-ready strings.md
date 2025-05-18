04-01-2025
When we run this command:
python manage.py makemessages -l pl -d djangojs
It takes not only .js files created by us but also those from other static .js files, like admin, or the i18n_catalog: 
```
./cal_env/lib/python3.12/site-packages/django/views/templates/i18n_catalog.js
```
And this gives us errors. So there are two solutions for it. Either exclude the problematic files with --exclude, or go to the exact directory in which we have our .js files to be translated, and run the command there. For aerial calendar, I went with the first option.



### Hashtags:


### References (source material, similar notes):
