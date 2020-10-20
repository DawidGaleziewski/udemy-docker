containers are immutable
This fallows 'immutable infrastructure' pattern. containers are re-deployed and never changed

# persistant data
there is a issue with persistant data that we want to tackle when we store info like database data.

Docker have two solutions for this issue:

## data volumes
Volumes are separate directories that are allowed to change

## Bind mounts
paths outside the container to the localhost