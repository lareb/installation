

**Installation of Nginx on Ubuntu (Docker)**
========================================

Nginx (pronounced engine x) is a lightweight, free, open-source HTTP and reverse proxy server, as well as a mail proxy server. The Nginx project started with a strong focus on high concurrency, high performance and low memory usage.It is one of the most popular web servers in the world and is responsible for hosting some of the largest and highest-traffic sites on the Internet. It is more resource-friendly than Apache in most cases and can be used as a web server or a reverse proxy.

Pull the Nginx image file from the docker hub
--------------------------------------------
```
$ sudo docker pull nginx
```

To run Nginx while binding the guest port 80 to the host port 80
-------------------------------------------------------------
```
$ sudo docker run --name docker-nginx -p 80:80 nginx
```

To run it in the background add -d
-------------------------------
```
$ sudo docker run --name docker-nginx -p 80:80 -d nginx
```

check if it is running run
--------------------------
```
$ docker ps -a
```

To Stop Nginx run
-----------------
```
$ docker stop docker-nginx
```

Remove the container
--------------------
```
docker rm docker-nginx
```
