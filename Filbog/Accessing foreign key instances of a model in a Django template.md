
Example case: I'm on a article_list template, so my main model would be article. But I want to display all the comments under specific articles.
https://docs.djangoproject.com/en/4.2/topics/db/queries/#following-relationships-backward - using entry_set to get those, and then we can use a loop or whatever we need in a specific case. In the template, the code would look sth like this:
```
{% for comment in article.comment_set.all %}
	<code>
{% endfor %}
```


#django #djangomodels #webdev #coding