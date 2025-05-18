09-01-2025

### Django docs
https://docs.djangoproject.com/en/5.1/topics/i18n/translation/
Everything is basically here, even tho it's basically a book-amount of text

### most important commands
##### Create strings to translate:
```zsh
python manage.py makemessages -l pl
```
In Django, English is default. The last "pl" thing is a language code, we ofc change the output language code depending on our needs.
##### To create translated text from external .js files:

```zsh
django-admin makemessages -d djangojs -l pl
```
 Warning - there are lots of steps to actually get the external .js files translated. For example, we have to modify our project-level urls.py file to get the gettext function working in those. Also, I was getting lots of errors when trying to get this command working from project-level directory. There are two solutions:
 - Go to your parent .js files directory and run the command from there (didn't test it)
 - Exclude certain folders, like here:
```zsh
python manage.py makemessages -l pl -d djangojs --ignore="*/admin/*" --ignore="node_modules/*" --ignore='*/i18n_catalog.js'
```
To "compile" the strings from .po file/s to be displayed in our project:
```zsh
python manage.py compilemessages
```
### Example Project
https://github.com/Filbog/aerial-calendar 


### Hashtags:
#translation #localization #internationalization #coding #webdev #django

### References (source material, similar notes):
Useful StackOverflow threads:
   - https://stackoverflow.com/questions/67511278/how-to-solve-the-translation-localisation-of-javascript-external-files-since-dja
   - https://stackoverflow.com/questions/71757020/how-to-translate-text-in-an-external-javascript-file-django/71757782#71757782