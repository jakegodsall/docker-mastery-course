# `docker-compose.yml`

## Definition

A YAML file used with Docker Compose to define multi-container application environments

#### Versions

-   Version 1: Lacks many of the networking and volume features introduced in later versions.
-   Version 2: Introduced support for multiple networks and volumes.
-   Version 3: Focuses on cloud and orchestration compatibility, especially for Docker Swarm.

#### Keys

-   `version`: Specifies the version of the Docker Compose file format.
-   `services`: Defines the different containers that make up the application.
-   `networks`: Specifies the networks to be created and used by the containers.
-   `volumes`: Defines the volumes to be created.
