# Volumes Cheatsheet

## Creating Volumes

Craeting a volume:

```bash
docker volume create [VOLUME_NAME]
```

## Deleting Volumes

Delete a volume by volume id:

```bash
docker volume rm <volume_id>
```

Delete all volumes that are not currently in use by a container:

```bash
docker volume prune
```

Delete all volumes (forced):

```bash
docker volume rm $(docker volume ls --quiet)
```
