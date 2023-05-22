# WorkShop MicroService Spring boost using Docker

## Docker Image
Using Image From [docker image](https://hub.docker.com/_/eclipse-temurin)
## Command Docker
Build image 

        docker image build -t spring:1.0 .

Create Container 

        docker container run -d -p 9999:8080 spring:1.0
        * run on port 9999 call container port 8080 *

## Build Docker Multi Stage Image
Build image

        docker image build -t springdemo2:2.0 -f Dockerfile_multi_stage .

## Docker compose 
1. Create file `docker-compose.yml` 
2. Build image

        docker compose build
3. Run Container

        docker compose up -d
        docker compose ps <*list all container running*>
4. Remove all containers

        docker compose down <*shut down*>
