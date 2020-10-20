Each container connect to private network bridge

Netowrking fallows bateries included but removable. Where default settings work well but we can mod them

We can:
 - make new virtual networks
 - attach docker containers to more the one
 - ship virtual neworks and use host ip --net=host

 # To check container ip

 docker container inspect --format '{{ .NetworkSettings.IPAddress}}'