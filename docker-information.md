<!-- TITLE: Docker Information -->
<!-- SUBTITLE: A place to put notes about Docker that I have learned from the pre-reqs -->

# Useful Docker Commands
## Run a docker container with a given name.
### docker run -d --name="*name*" *imagestore*/*imagename* 
## Tail the stdout of a running container specified by the given name
### docker logs -f *name*       (Tails the stdout of the container)