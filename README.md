# docker-and-kubernetes

## Basic command
### Run container
```bash
docker run --p 80:80 nginx
```
Another options:

> * -d: detach process
> * --name: give name to the container
> * --net: network for the container
> * -e: set env variable

### Stopping container
```bash
docker stop {container_id}
```

### Get list of active containers
```bash
docker container ls
```
another options:
> * -a: get all containers

### Show docker container logs
```bash
docker container logs {container id}
```

### Show running process on the container
```bash
docker container top {container_id}
```

### Deleting container
```bash
docker container rm {container_id}
```
another options:
>* -f: force delete even if the container is running

---

### Inspecting container
```bash
docker container inspect {container_id} bash
```
### Resource monitoring in container
```bash
docker container stats
```
---
### Attach shell to new container
```bash
docker container run -it {docker_image/container}
```

### Attach shell to running container
```bash
docker container exec -it {container}
```
--------
## Netowrking
### Show port of a container
```bash
docker container port {container}
```

### Show all networks
```bash
docker network ls
```

### Inspect docker network
```bash
docker network inspect
```

### Attach running container to network
```bash
docker network connect {network} {container}
```

### Dettach running container from network
```bash
docker network disconnect {network} {container}
```
