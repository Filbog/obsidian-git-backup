#coding #docker #djangoforprofessionals 


A ***Docker image*** is a read-only template that describes how to create a ***Docker container.*** The image is the **instructions** while the container is the **actual running instance of an image**. To continue our apartment analogy from earlier in the chapter, an image is the blueprint or set of plans for building an apartment; the container is the actual, fully-built building.
Images are often based on another image with some additional customization. For example, there are "base" images for Python that we built our own images on top of.

To run the Docker container, we run command *docker compose up*

Instructions for how to create our image are in **Dockerfile**, whereas instructions for the container are in **docker-compose.yml**.


