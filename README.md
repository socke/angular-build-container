# Angular Build container
This is a simple angular building container for angular projects. 

## Howto

### Folders

**/nginx** folder holds the nginx config file. Will be copied to the docker container later. 

### Dockerfile

The dockerfile uses a multi-stage-build (new since docker 17.x) where the angular app will be build inside the first build stage and then the next image will run an nginx image with the created application. 
