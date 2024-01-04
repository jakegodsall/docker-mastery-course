# Docker Swarm Cheat Sheet

## Initialise a Swarm Cluster

Converts the Docker engine running on the current node into a swarm manager node:

```bash
docker swarm init
```

## Managing Swarm Nodes

List all nodes in the swarm:

```bash
docker node ls
```

Get detailed information about a specific node:

```bash
docker node inspect <NODE_ID>
```

Remove a node from the swarm:

```bash
docker node rm <NODE_ID>
```

Update the role of a node in the swarm:

```bash
docker node update --role manager/worker <NODE_ID>
```
