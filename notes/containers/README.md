# Containers

### Definition

A container is:

-   a sandboxed process on your machine that is isolated from all other processes.
-   a runtime instance of an image.

### Properties

#### Location

Containers are stored on the filesystem of the host:

-   Linux: `/var/lib/docker/containers`.
-   Windows: Stored within the WSL2 (not directly accessible by the Windows host in a simple file path).
-   macOS: Stored in a Linux VM managed by Docker Desktop.

#### Immutability

Docker containers are immutable by design, not by requirement. This makes them more consistent, reliable, and predictable.

Advantages:

-   Can be sure that a container will run the same everywhere, be it your local machine or in production.
-   Has the added benefit of tying in well with the design philosophy of version control systems.

#### Ephemerailty:

Docker containers can be started, stopped, and destroyed quickly.

Advantages

-   Can be created when needed, and destroyed when their task is complete, leading to efficient resource allocation.
-   Ideal for experimentation because you can start and stop different containers quickly.
