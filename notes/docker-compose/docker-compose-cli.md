# Docker Compose Command Line Tool

## Definition

The Docker Compose command-line tool is a utility to manage the lifecycle of multi-container Docker applications.

### Life Cycle Management

Create and start all containers defined in the `docker-compose.yml`:

```bash
docker compose up
```

The `-d` option can be added to run the containers in the background.

Stop and remove the containers, networks, and volumes created by `docker compose up`

```bash
docker compose down
```

Build/rebuild the services specified in the `docker-compose.yml` file that have a build context.

```bash
docker compose build
```
