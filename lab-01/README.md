
https://labs.play-with-docker.com

https://hub.docker.com/_/nginx/

docker pull nginx

docker run -itd -p 80:80 nginx

docker ps

docker rm [name / id]

mkdir /root/web
vi index.html 
<html>
    <body>
        <h1>My Web1</h1>
    </body>
</html>

docker run -itd -p 80:80 -v /root/web:/usr/share/nginx/html nginx
http://ip172-18-0-11-bb019gdeoia0009n7m3g-80.direct.labs.play-with-docker.com



