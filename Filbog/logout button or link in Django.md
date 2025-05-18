#coding #django #webdev 

logout must always be a POST request in Django - so we can' just do a button or a HTML tag with a URL. Has to be something like this:

```
<p><form action="{% url 'logout' %}" method='post'>

{% csrf_token %}

<button name='submit' class='btn btn-outline-secondary btn-sm'>

Log out</button>

</form></p>
```