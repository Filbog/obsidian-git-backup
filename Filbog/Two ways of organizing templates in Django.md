#coding #django #webdev #backend 

1. Default - in each app dir, create a directory called *templates* and a nested *app_name* directory within.
2. Project-level directory - create *templates* in the root directory. Then in *settings.py* modify the *TEMPLATES* object, *DIRS* attribute:

	```
	TEMPLATES = [  
    {
	    "DIRS": [BASE_DIR / "templates"], 
	}  
	]
```
