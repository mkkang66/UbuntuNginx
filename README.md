# dockerfiles-centos-user-adderable
Centos7, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build --rm -t mkkang66/ubuntu_nginx .
	docker run -it --name u1 -v c:\\Users\\user\UbuntuNginx:/var/www/html mkkang66/ubuntu_nginx
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
ad2ad96e4b2f        mkkang66/ubuntu_nginx      "/bin/bash"         7 seconds ago       Up 6 seconds                            c1
```

To test, ("nowage" is username. )
```
	~~~~~~
```
To Rollback
```
    docker rm c1 -f
    docker rmi mkkang66/ubuntu_nginx
```
