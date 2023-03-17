# DOCKER

## Overview
This is the minimum required code example for using reproducing a docker container. The container will contain a server we have built which simply listens to the PORT 8080.

## Instructions
Use the docker build command in the root directory to create an image of the server we have built.
```
docker build -t tag_name
```
This produces a docker image for the given code with the name tag_name and you will receive a container_id for the same.
Then, to run the container, use the docker run command.
```
docker run -p 5000:8080 container_id
```
This will run the container, and will forward its virtual port (8080, in this case), to the port 5000 of our local machine, so that we can actually access it.