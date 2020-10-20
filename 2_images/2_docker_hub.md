# official images
official images wont have forward slash in front of them i.e
nginx
nginx/dawidgaleziewski
nginx/ivanti

## check downloaded images
docker image ls

## tags
latest - latest version of this product. Most current version

i.e if we run
docker pull nginx - it will download the lates image

to download specific version
docker pull nginx:1.11.9
We can use any other tag on dockerhub i.e mainline

in production we would like to download specific tag version

alpaine - small distro of linux. Some images have multi distro versions