
It's important for performance reasons (Docker is caching files to make future builds faster). So, "in order to avoid constantly invalidating the cache we start the Dockerfile with commands that are less likely to change while putting commands that are more likely to change, like COPYing the local filesystem, at the end." - from Django for Professionals

#coding #docker #webdev #djangoforprofessionals