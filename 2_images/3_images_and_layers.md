# image layers
Images are designed using union file system.
That is making layers of changes


docker history <image name>
Every image starts with a scratch.
Every change that happens on file system is another layer

when we start a image we start with first layer
 
 each layer gets another sha i.e

Example of image and its layers:
 [ENV variable change]
 [Docker file with another file]
 [UBUNTU]


 Another image
 [OPEN PORT]
 [COPY file]
 [APT]
 [DEBIAN]

 Layers we have like debian image or same open ports changes will be cached. So we do not need to download them again

 Docker stores each layer on same level only once

 If we change even one line of code on a layer we will create a new image.

 When we run a container from a image. The image files are read only. 

 Copy on write - when we change image files in container. What happens is that container changes them in container layer and not image itself

 we can see the changes on the layer in docker image history

 # docker image inspect
this is info on metadata of the image on how it suppose to run

