# Docker

## Basic commands
### General
```sh
# Lists running containers
$ docker ps

# Lists all containers
$ docker ps -a

# Removes a container
$ docker rm <container_id>

# Removes all stopped container
$ docker container prune

# Remove stopped containers by filters
$ docker container prune --filter status=exited --filter "until=12h"

# Lists images
$ docker images

# Removes an image
$ docker rmi <image_id> 
```

### On project
- On project root
```sh
$ docker build . -t myproject:1.0 # Build via Dockerfile to create a Docker image
```

- Access interactively to Docker container with image named "myproject" with tag 1.0 and run command "/bin/sh" to start a shell terminal session
```sh
$ docker run -it myproject:1.0 /bin/sh
```

## Dockerfile

## Docker compose
