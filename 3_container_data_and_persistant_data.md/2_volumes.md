to specify volume in our dockerfile we put

VOLUME /var/lib/mysql

Volumes need manual deletion.
It requires additional step to be deleted

When we use mysql image for example and enter a running container json metadata of it:
docker container inspect mysqlname

we will se unde rmount that it has a source on our localhost

We can list volumes by
docker volume ls

we can specify a volume
docker container run -d --name mysql -e MYSQL_ALLOW_EMPTY_PASSWORD=True -v mysql-db:/var/lib/mysql mysql