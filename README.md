### docker-lab ###

#1 Register 
https://hub.docker.com

#2
https://labs.play-with-docker.com

#3
git clone https://github.com/MoccaMc/docker-lab.git

## fetch
git fetch origin master

## merge
git merge origin/master

##Docker Swarm
docker swarm init --advertise-addr 192.168.0.26

docker swarm join --token SWMTKN-1-48frkcbzwyuh9oipz98ry87gghtu902ne4rifspet8j4uiabwi-6vxptxljuzujvr4a0v832de7e 192.168.0.26:2377

docker node ls

docker node promote node2

