docker container run -it nginx bash
t stends for TTY which is a open session
i stands for interactive. It keeps the session opened

After the image name we add arguments for that image. So we can open bash on start


## To start new container interactively:
docker container run -it

## To run additional command with the container
docker container exec -it

## Starting existing container with terminal
docker container start -ai <id>

Important to know is that if the image does not have bash we cannot connect to it. We cannot run a program inside a container if it does not have it. For example

docker pull alpine
docker container run -it alpine bash

It will thor a error

We can however use docker run -it alpaine sh