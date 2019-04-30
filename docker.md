# Docker

# Basic commands
## General
```sh
$ docker ps # Show all running containers
$ docker images # Show all local images
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

