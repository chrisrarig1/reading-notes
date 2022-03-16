# Django REST Framework & Docker

- Docker is a way you can isolate and run entire applications

## Install Docker

- Install desktop app at docker.com/get-started
- Install Docker Compose: `sudo pip install docker-compose`
    - This is automatically included in Windows and Mac downloads of docker
- Check if the install worked with these commands:
    - `docker --version`
    - `docker-compose --version`
    - `docker run hello-world`
    - `docker info`

## Images and Containers

- An *Image* is a snapshot of what the project contains
- A *Container* is a running instance of the image

## Local Image/Containers

- In your project add Dockerfile: `touch Dockerfile`
- Add file for containers instructions: `touch docker-compose.yml`
- Code Example:
    - `From: image`
    - `ENV: environment variable`
    - `WORKDIR: working directory`
    - `COPY: copy dependencies lock file RUN: installation of dependencies`
    - `COPY . /code/ : copy project`

# Useful Links

- [A Beginner's Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)
- [Django for APIs](https://djangoforapis.com/library-website-and-api/)