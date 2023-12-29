# Using Bind Mounts

The following directory defines a `Dockerfile` for an nginx server, which hosts a single HTML file called `index.html`.

It is used to demonstrate how to use bind mounts for development purposes.

The command to create the appropriate container with the bind mount is:

```bash
docker container run --publish 80:80 --name nginx --detach --volume $(pwd):/usr/share/nginx/html nginx
```
