# tags
images do not really have a name.
We eaither do by repository 

Tag is not a version or a repo. It is similar to git repo tag. It is a pointer to specific commit

Same image id may have multiple image IDs

we can re-tag the image name by:
docker image tag nginx dawidgaleziewski/nginx

we can push the image by docker image push <tag>

We can add multiple tags like

docker image tag nginx nginx:testing