
https://labs.play-with-docker.com

https://hub.docker.com/_/nginx/

git clone https://github.com/MoccaMc/docker-lab.git
cd ~/docker-lab/lab-01/

docker pull nginx

docker run -itd --name my-nginx -p 9901:80 nginx:1.13.10-alpine

docker run -itd --name my-httpd -p 9902:80 httpd

docker run -itd --name my-tomcat-8 -p 9903:8080 tomcat:8.0

docker run -itd --name my-tomcat-9 -p 9904:8080 tomcat:9.0.14-jre11-slim

docker ps

docker rm [name / id]

docker run -itd --name ngx1 -p 81:80 -v /root/docker-lab/lab-01/web1:/usr/share/nginx/html nginx

docker run -itd --name ngx2 -p 82:80 -v /root/docker-lab/lab-01/web2:/usr/share/nginx/html nginx:1.13.10-alpine

docker images

docker ps -a

docker stop [name / id]

docker stop $(docker ps -a -q)

docker start [name / id]

docker rm -f $(docker ps -a -q)

index.html 

<html>
    <body>
        <h1>My Web1</h1>
    </body>
</html>

