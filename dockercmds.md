
# docker imp commands 

```

$ docker info
$ docker images
$ docker rmi <imagename>
$ docker pull <imagename>
$ docker run <imagename>
$ docker run -d -p host-port : container-port <image-name>
$ docker tag <image-name> <image-tag-name>
$ docker login
$ docker push <image-tag-name>

$ docker ps
$ docker ps -a
$ docker stop <container-id>
$ docker rm <container-id>
$ docker rm -f <container-id>
$ docker system prune -a
$ docker logs <container-id>
$ docker exec -it <container-id> /bin/bash

$ docker network ls
$ docker network create <network-name>
$ docker network rm <network-name>
$ docker network inspect <network-name>

$ docker-compose up -d
$ docker-compose down
$ docker-compose ps
$ docker-compose images
$ docker-compose stop
$ docker-compose start

$ docker volume ls
$ docker volume create <vol-name>
$ docker volume inspect <vol-name>
$ docker volume rm <vol-name>
$ docker system prune --volumes


$ sudo docker service --name <service-name> -p 8080:8080 <img-name>
$ sudo docker service scale <service-name = replicas
$ sudo docker service ls
$ sudo docker service rm <service-name>
```






---




# docker imp unique commands 

```
docker build --platform linux/amd64 -t akshay0909/sam:2.0.bymac .
docker run --platform linux/amd64 --name samplecont -d -p 8080:8080 akshay0909/samplemaven:2.0 
```


---


docker port <containerid>
docker diff <containerid>
docker wait <containerid>
docker kill <containerid>
docker attach <containerid>
docker cp <containerid>:<source> <destination>
docker history <imagename>
docker logs -f <containerid>
docker stop $(docker ps -q)
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
docker-compose restart
docker-compose rm
docker-compose build
