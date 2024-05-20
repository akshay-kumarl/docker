## might be usefull docker commands


```
1. docker search image-name :- Finding out an image from Dockerhub.io.
2. docker info :- Docker Engine all info end to end basis .
3.Docker pull :'- Docker image pull from registry
4.docker run :- Create a new container from the Docker images .
5.docker logs container-id :- Check any container logs for debugging and monitoring
6. docker history image-name :- It ideally contains all configuration files and it will also show how all Docker file commands to spin up the container .
7.docker ps -a :- Listed all Docker containers
8. docker exec -it container-name /bin/sh :- It opens in a interactive shell & execute commands in container itself rather than in Docker daemon .
9. docker kill :- Kill one or more containers
10.docker stop :- Stopped the containers functioning
11.docker network ls :- List down all existing & created networks in Docker
12.docker network inspect network-name:-Inspect any existing docker network
13.docker push tagged-image-name :- Post tagging an image push it in our local Docker hub
14.docker rmi :- Remove one or more images .Easy to remember the last word with i .
15. docker rm :- Remove one or more containers
16.docker rename old_container_name new_container_name :- Rename an existing container
17.docker pause container_ID_or_name :- Pause an docker one or more containers.
18.docker unpause container_ID_or_name :- Unpause or restart on e or more Docker containers
19.docker port container_ID_or_name :- View the existing ports .
20.docker diff container_ID_or_name :- Inspect changes of files & directories on a container's file system .
21.docker top container_ID_or_name :- To see current memory & CPU utilization .
22. docker stats :- Monitor the Docker Memory , CPU & ongoing processes inside Docker .
23. docker login & logout :- Login to Dockerhub.io and Logout accordingly
24. sudo usermod -a -G docker $USER :- Add an user to Docker group to avoid root privileges 
```
