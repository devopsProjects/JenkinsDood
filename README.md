# JenkinsDood
jenkins image for Docker Outside Of Docker

This image is useful when Jenkins running inside a docker container needs to access the host docker

How to run
docker run -d --name jenkins_dood -p 49001:8080 -v /data/jenkins_home:/var/jenkins_home:z -v /var/run/docker.sock:/var/run/docker.sock -v $(which docker):/usr/bin/docker-t kannach/jenkinsdood:1.9.0

volumes to mount

jenkins data driectory
docker socket
docker executable
