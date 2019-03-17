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
	

docker run busybox ls

## 
docker ps
docker ps --all 

## create a containner 
docker create hello-world
docker  start -a 9f0bbb30d680912cbb211af2dea4390c9399c749d10c566cc1d6bf9cdffec2b4


docker system prune

## Logs
docker logs a54771304d4653048d1358509d2062bb27da9c9b1395d9f6c398882dbc1f20a7

docker stop 90aafd48c33f 
docker kill 90aafd48c33f 



docker pull redis:latest
docker run redis
docker exec -it f307b9924184 redis-cli
docker exec -it f307b9924184 sh

docker run -it busybox sh



dockerer build .
docker build -t panterha6/redis:latest .


docker commit -c 'CMD ["redis-server"]' f307b9924184

docker run -p 8080:8080 panthera6/simpleweb:0.01
docker build -t panthera6/simpleweb:0.01 .

docker-compose up
docker-compose up --build

# background
docker run -d redis

docker-compose up -d
docker-compose down

docker-compose ps


