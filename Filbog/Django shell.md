
#coding #webdev #django 

accessing Django shell: ***python manage.py shell***
It's a Python interpreter so we can put there basically any Python/Django code and it should work. We can assign variables, do loops etc
When we for example have a Topic model and want to display all its instances in terminal:
	*from <app_name>.models import Topic*
	*Topic.objects.all()*
To see IDs of all our topics:
	*topics = Topic.objects.all()*
	*for topic in topics:*
		*print(topic.id, topic)*

To exit on Mac: **ctrl + D**

[Creating db queries in Django](https://docs.djangoproject.com/en/5.0/topics/db/queries/)
