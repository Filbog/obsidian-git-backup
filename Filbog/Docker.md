Docker helps, most of all, in having the same environment - python version, django or other services - across all computers and/or operating systems. Docker is a container for that stuff - so everything is running within Docker itself.
Docker *isolates* an entire operating system via Linux containers - but it's a mini operating system, only with the stuff necessary to run our thing.

Via ***Django for Professionals:***
"Docker also makes collaboration in teams exponentially easier. Gone are the days of sharing long, out-of-date README files for adding a new developer to a group project. Instead with Docker you simply share two files–a Dockerfile and docker-compose.yml file–and the developer can have confidence that their local development environment is exactly the same as the rest of the team."
"An analogy we can use here is that of homes and apartments. Virtual Machines are like homes: stand-alone buildings with their own infrastructure including plumbing and heating, as well as a kitchen, bathrooms, bedrooms, and so on. Docker containers are like apartments: they share common infrastructure like plumbing and heating, but come in various sizes that match the exact needs of an owner."

What's also awesome is that Docker container can be very easily ***synced*** via the **volumes mount** in docker-compose.yml:"
Finally the [volumes](https://docs.docker.com/storage/volumes/) mount automatically syncs the Docker filesystem with our local computer’s filesystem. This if we make a change to the code within Docker it will automatically be synced with the local filesystem."
Example in [this repo](https://github.com/Filbog/django-for-pros-ch4) or any repo from Django for Pros for that matter.


#coding #docker #djangoforprofessionals