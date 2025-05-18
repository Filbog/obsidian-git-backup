Official Django docs even recommend this, even if we're OK with just using the basic User model at the moment. Why? Because after running first *migrate*, modifying it will be an extreme pain in the ass. 
Here we're extending ***AbstractUser*** to "create a custom user model that behaves identically to the default User model but provides the option for customization in the future" via Django for Beginners (the Pros version too). Docs propose working with ***AbstractBaseUser***, but according to book's author, this is more complicated and reduntant for most cases - touching *AbstractBaseUser*, we're rewriting core Django code. If we just want some additional fields for the user model, it's better to use *AbstractUser*. If we need even more flexibility the AbstractBaseUser provides, it can be added later.

 - **Important to create the custom user model before running *migrate*** for the first time
4 steps for creating the custom model:
 -  create a new *CustomUser* model (preferrably create a new app for this)
 - update *django_project/settings.py* - add the app and *AUTH_USER_MODEL = app.CustomUserModel*
 - create new forms for *UserCreationForm* and *UserChangeForm* - this one's for the admin panel
 - update *accounts/admin.py* - same as above, for admin panel

Example for all those steps and created custom user - https://github.com/Filbog/django-for-pros-ch4
[Referencing our custom User model](https://docs.djangoproject.com/en/5.0/topics/auth/customizing/#referencing-the-user-model)


[[null VS blank in Django models]]
#django #coding #webdev #djangoforprofessionals #django