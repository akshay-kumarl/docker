# Docker
this repo contains docker-related notes and files.

**DOCKER ARCHITECTURE** 
![Architecture-of-Docker](https://github.com/akshay-kumarl/Docker/assets/110522215/6eefab69-2125-4e45-8927-d7f31324cb14)


### Docker Related important links

---

### docker portainer 

```
docker create volume create portainerdata

docker run -d -p 8000:8000 -p 9443:9443 --name portainer \
        --restart=always \
        -v /var/run/docker.sock:/var/run/docker.sock \
        -v portainer_data:/data \
        portainer/portainer-ce:2.11.1

```
