2024-08-10


It’s important to be aware that Git, by default, will not track directories that are empty. Thus when we eventually push our code to both GitHub and Heroku these empty directories will not appear which can cause problems in deployment when collectstatic is run. To avoid this we can add an empty file. like ***.keep*** to the folder

### Hashtags:
#coding #git #djangoforprofessionals #deployment 


### References (source material, similar notes):
