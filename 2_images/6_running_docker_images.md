We first need a dockerfile

Secondly we need to run:
docker image build -t customnginx .
(-t stands for tag)

It will pull the distro and run all stanzas and cache each layer

now we should be able to see docker image in ls


It is important to keep things that change the least on top of the docker file. And the things that change the least on bottom of it

# clean up builds and containers
docker system prune