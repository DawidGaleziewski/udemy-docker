- docker container run will try to run a image stored locally.

- If it does not find one it will jump to the docker hub (online)

- Docker will create new container basing on image and prepers to start

- gives the container a virtual ip on a private network inside docker engine

- opens specified port on host and forwards it to port on docker

It will use a lot of defaults if we do not dpecify those on our command