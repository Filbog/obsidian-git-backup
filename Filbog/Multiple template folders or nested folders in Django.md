
Example: [Timeaware repo.](https://github.com/Filbog/timeaware-django)
In templates folder, I also have a **nested** errors folder, for error templates. The template won't 
work out-of-the-box, we have to set a new folder in settings.py:
```
"DIRS": [BASE_DIR / "templates", BASE_DIR / "templates/errors"],
```
So here, "templates" is the default folder - Django will look there for the template. If it doesn't find matching template, then it looks in the nested "errors" folder.


#coding #webdev #django #backend