# Image vs Container

## image is:
Binarys and source code making application

## container 
instance of the image. There may be multiple running containers of same images


# Running a container
To run a generic nginx container:
docker container run --publish 80:80 nginx

1. Docker looks for a image called nginx
It downloaded it from docker hub


As we do not wat it to run in command line all the time
docker container run --publish 80:80 --detach nginx

each time we run a container we get its unique id:
441d388207b6c785d37ccfb7b8d360f5eae7aae6551320df5a691dc006909500

# stopping container
we can stop it with:
docker stop <id>
we can only write first digits so that container is unique to stop it

# listing containers
docker container ls

Name and id are required. If we do not do this it will be auto generated

# baning container
docker container run --publish 80:80 --detatch --name webhost nginx

# checking logs from a container
docker container logs <name>


# check processes running inside the container
docker container top <name>

# remove container
docker container rm <id>
docker container 934 923 6jd

if the container is running
docker container rm -f <id>

## useful options
-e for enviroment
-d for detach
-p publish ports to the host
