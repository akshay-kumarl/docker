# Docker
this repo contains docker-related notes and files.

**DOCKER ARCHITECTURE** 
![Architecture-of-Docker](https://github.com/akshay-kumarl/Docker/assets/110522215/6eefab69-2125-4e45-8927-d7f31324cb14)


### Docker Related important links

---

### Docker portainer  (visual viewer)

```
docker create volume create portainerdata

docker run -d -p 8000:8000 -p 9443:9443 --name portainer \
        --restart=always \
        -v /var/run/docker.sock:/var/run/docker.sock \
        -v portainer_data:/data \
        portainer/portainer-ce:2.11.1

```

---

### Topics to cover in docker

Week 1: Docker Foundations

- Introduction to Containers
- Docker Architecture & Lifecycle
- Why Docker is Popular
- Build, Ship, Run!

Dive Deeper:

- Containers vs Virtual Machines
- Files & Folders in Containers
- Docker Terminology & Installation
- Writing My First Dockerfile

Week 2: Advanced Docker Concepts

- Multi-Stage Docker Builds
- Distroless Images & Benefits
- Containerization of Django Application
- Containerization of Python Application
- Reducing Image Size Significantly

Networking Deep Dive:

- Container to Container Communication
- Container to Container Isolation through Custom Bridge
- Bridge vs Host vs Overlay Networks
