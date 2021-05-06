runing
------

docker run -d -t --name server72 --mount type=bind,src=/home/defyma/web_56/,dst=/opt/app-root/src -p 8080:8080 defyma/s2i-php72-pdoocirfc /usr/libexec/s2i/run

cek container "server72" is running, locahost:8080 is up
-------------
docker ps -a

start/stop
----
docker start server72
docker stop server72

enter bash
----------
docker exec -it server72 bash
