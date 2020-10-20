# Docker file
It is like a recepie for a image
It may look like a shell script but it is not. It is its own lang.

Dockerfile usually starts with FROM command specifying which distro is used. I.e:

# DOCKERFILE stanza
Each is a layer.
Order of those matters
Here we use for example apt get to install new packages.

Good practice is to chain commands so that it stays one layer. This will save time i.e:

RUN apt-get update \
	&& apt-get install --no-install-recommends --no-install-suggests -y gnupg1 \
	&& \


## Second part is usually for logs
RUN ln -sf /dev/stdout /var/log/nginx/access.log \
	&& ln -sf /dev/stderr /var/log/nginx/error.log

Errors are put usually in stdout or stderror for docker builds

# FROM
FROM debian:stretch-slim

We use package managers like apt or yum to build images

# ENV
enviroment variables. They are very important as they are used to insert keys and values to run docker with them.

# EXPOSE
What ports will be opened from the container to outside. Does not MEAN this will be opened automatically on our host. This is NOT --publish command that is exposing ports to the host.

# CMD
final command run when we start a new container from a image

# WORKDIR
it is better to use workdir when changind directory then to use run and then cd

# COPY
When copying something to the docker from local device

