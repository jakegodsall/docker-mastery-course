# Volumes

### Definition

A volume is:

-   The preferred mechanism of persisting data in Docker.

### Properties

#### Location

Volumes are stored on the filesystem of the host:

-   Linux: `/var/lib/docker/volumes`.
-   Windows: Stored within the WSL2 (not directly accessible by the Windows host in a simple file path).
-   macOS: Stored in a Linux VM managed by Docker Desktop.

#### Independent Lifecycle

The lifecycle of a volume is indepenedent of that of a container, meaning that the volume's data can be persisted after the corresponding container has been destroyed.

### Types

#### Anonymous Volumes

##### Definition

A volume created without a specific name.

##### Use Case

Useful for temporary or throwaway data that does not need to be named or persisted.

#### Named Volumes

##### Definition

Volumes created with a specific name.

##### Use Case

Used for persisting data and sharing it between containers or between a container and the host.

#### Bind Mounts

##### Definition

A link to a specific filesystem path on the host to a path in the container.

##### Use Case

Bind mounts allow for real-time synchronisation between the container and the host system, which is useful for active development or testing.