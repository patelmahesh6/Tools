Docker is a platform for developers and sysadmins to develop, deploy, and run applications with containers.

A container is launched by running an image. An image is an executable package that includes everything needed to run an application–the code, a runtime, libraries, environment variables, and configuration files.

A container is a runtime instance of an image–what the image becomes in memory when executed (that is, an image with state, or a user process). 

***************


## List Docker CLI commands
docker
docker container --help

## Display Docker version and info
docker --version
docker version
docker info

## Excecute Docker image
docker run hello-world

## List Docker images
docker image ls

## List Docker containers (running, all, all in quiet mode)
docker container ls
docker container ls --all
docker container ls -a -q


