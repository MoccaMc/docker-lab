
https://labs.play-with-docker.com

https://hub.docker.com/_/nginx/

git clone https://github.com/MoccaMc/docker-lab.git
cd ~/docker-lab/lab-01/

docker pull nginx
docker run -itd -p 80:80 nginx
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

