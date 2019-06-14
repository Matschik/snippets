# Docker

## Basic commands
### General
```sh
# Removes all stopped container
$ docker container prune

# Remove stopped containers by filters
$ docker container prune --filter status=exited --filter "until=12h"
```

### On project
- On project root
```sh
$ docker build . -t myproject:1.0
```

- Access interactively to Docker container and run command "/bin/sh" to start a shell terminal session
```sh
$ docker exec -it myproject:1.0 /bin/sh
```

## Dockerfile

## Docker compose
