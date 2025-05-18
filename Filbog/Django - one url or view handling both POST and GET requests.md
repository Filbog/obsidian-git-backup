

Example: we have a DetailView, but want a form to add a new entry or whatever. 
**In function views**, we can always do if request == POST etc, and/or break GET and POST request handlers into two different functions, like in the [Learning Log project](https://github.com/Filbog/learning-log)
It's a different story with **class-based views** tho. In views.py in [TimeAware project](https://github.com/Filbog/timeaware-django), we have a ListView connected with a form to add new shit

