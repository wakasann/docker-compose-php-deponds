only base on `php7.1-apache`,run laravel 5.4 project

redis,mysql, use [sprintcube/docker-compose-lamp](https://github.com/sprintcube/docker-compose-lamp) run container


------------


```
sudo docker pull centos:6.10

sudo docker run -s="devicemapper" --name=centos610 -p 8089:80 -d -i -t centos:6.10 /bin/bash 

sudo docker exec -it centos610 bash
```


try commonds:

```
yum -y update
yum install -y net-tools epel-release autoconf automake vim wget
yum install -y httpd
chkconfig httpd on
wget http://dev.mysql.com/get/mysql57-community-release-el6-7.noarch.rpm
rpm -Uvh mysql57-community-release-el6-7.noarch.rpm
vim /etc/yum.repos.d/mysql-community.repo
yum install mysql-community-server
```

can not run mysql server in docker this docker container
