# Container Cheatsheet

## Creating Containers

## Inspecting Containers

Determining the port numbers on the host and within the container:

```bash
docker container port CONTAINER
```

## Deleting Containers

Delete a single container

```bash
docker rm [CONTAINER_ID or CONTAINER_NAME]
```

Remove all stopped containers:

```bash
docker container prune
```

Force delete all containers:

```bash
docker container rm --force $(docker container ls --all --quiet)
```
