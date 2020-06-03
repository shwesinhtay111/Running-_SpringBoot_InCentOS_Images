# Spring Boot Web Application

##Part 6
This repository has the project files for the post SPRING BOOT WEB APPLICATION, PART 6 – SPRING SECURITY WITH DAO Authentication Provider
that is part of the tutorial series on Spring Boot available from by website at [Spring Framework Guru](https://springfrspringframework.guru)

## Checkout the full tutorial here!
[Spring Boot - making Spring Fun again!](https://springframework.guru/spring-boot-web-application-part-1-spring-initializr/)


CentOS Images Creation on docker
======================================
docker run -d centos

docker run -d centos tail -f /dev/null

docker ps


docker exec -it container-NAMES bash

whoami

ls

ps -ef

kill -9 1

ls

docker ps -e

ps -ef

java -version

yum install java


in terminal,

ls

ls -ltr

vi Dockerfile

docker build -t spring-boot-docker .

docker run -d -p 8080:8080 spring-boot-docker

docker ps

docker logs container_id

If you want to kill image,
docker kill container-Name container-id


Check Dockerfile include as follow:
----------------------------------------->>>>

FROM centos

RUN yum install -y java

VOLUME /tmp
ADD /spring-boot-web-0.0.1SNAPSHOT.jar myapp.jar
RUN sh -c 'touch /myapp.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/myapp.jar"]
<---end----->
