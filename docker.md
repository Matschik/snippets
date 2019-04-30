# Docker

# Basic commands
## General
```sh
$ docker ps # Lists running containers
$ docker ps -a # Lists all containers
$ docker rm <container_id> # Removes a container
$ docker container prune # Removes all stopped container
$ docker container prune --filter status=exited --filter "until=12h" # Remove stopped containers by filters

$ docker images # Lists images
$ docker rmi <image_id> # Removes an image
```

## On project
- On project root
```sh
$ docker build . -t myproject:1.0 # Build with Dockerfile to create a Docker image
```

- Access interactively to Docker container with image named "myproject" with tag 1.0 and run command "/bin/sh" to start a shell terminal session
```sh
$ docker run -it myproject:1.0 /bin/sh
```

