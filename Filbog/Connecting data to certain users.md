In web dev we need to connect the data to the user who submitted it. In most cases, we only need to connect the data highest in the hierarchy to a user, and the lower-level data will follow. For example, if in my **Learning logs*** app I have a Topic and there are many Entries for this Topic, we only need to connect the specific user to the Topic, and Entries will follow via the many-to-one relationship. In order to achieve this, we need to **add a foreign key relationship to a user** in our models.py:

`from django.db import models` 
`from django.contrib.auth.models import User`

`class Topic(models.Model):` 

`Text = models.CharField(max_length=200)` 
`date_added = models.DateTimeField(auto_now_add=True)` 
`owner = models.ForeignKey(User, on_delete=models.CASCADE)`
