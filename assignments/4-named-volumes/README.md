# Assignment 4: Database Upgrades with Named Volumes

### Requirements

1. Create a volume caleld `psql-data`

    ```bash
    docker volume create psql-data
    ```

2. Create a `postgres` container with version `15.1` using the named volume:

    ```bash
    docker container run --detach --name psql1 --env POSTGRES_PASSWORD=password --volume psql-data:/var/lib/postgresql/data postgres:15.1
    ```

3. Create a `postgres` container with version `15.2` using the named volume:.

    ```bash
    docker container run --detach --name psql2 --env POSTGRES_PASSWORD=password --volume psql-data:/var/lib/postgresql/data postgres:15.2
    ```

4. Check logs to validate.

    ```bash
    docker container logs psql1
    ```

    ```bash
    docker container logs psql2
    ```
