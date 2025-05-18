For example, in my repos working with Django for Pros, like [here](https://github.com/Filbog/django-for-pros-ch3) there are those two lines at the end of my docker-compose.yml:

```Dockerfile
volumes:
  postgres_data:

```
They create a **named volume** called postgres_data. Named volumes are created to **persist data** - if not saved/persisted, our data is removed when we're closing the Docker container. This persisted data can also be shared between services we've created with Docker.

**persistence via ChatGPT:** By using a named volume, the data stored in the volume will persist even if the PostgreSQL container is stopped or removed. This ensures that your database data is not lost when the container is restarted.

#coding #docker 