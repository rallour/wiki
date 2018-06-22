<!-- TITLE: Docker Information -->
<!-- SUBTITLE: A place to put notes about Docker that I have learned from the pre-reqs -->

# Useful Docker Commands
## Run a docker container with a given name with optional env variable passed into the image.
### docker run -d --name="*name*" [ -e *key*=*value*] *imagestore*/*imagename*  
## Tail the stdout of a running container specified by the given name
### docker logs -f *name*
## Delete a docker image
### docker rm -f *name*
## Inspect details about an image
### docker inspect -f '{{json .Mounts}}' *name* | jq
## Delete image from the docker registry
### docker rmi *image name*

