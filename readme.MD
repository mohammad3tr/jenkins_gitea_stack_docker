## gitea and jenkins via mounting docker.sock
- [x] ~~*Mounting the Docker Socket:  
Mounting the Docker socket (/var/run/docker.sock) into the Jenkins container,
effectively gives Jenkins full control over the Docker daemon on the host.
This means Jenkins has the same privileges as the host's root user, which can be a significant security risk, especially if Jenkins is compromised**~~ 

1- setup your mirror repository: 

 https://github.com/mohammad3tr/Docker-Registery.git

2- git clone https://github.com/mohammad3tr/jenkins_gitea_stack_docker.git 

3- docker build -t m3tr-jenkins -f Dockerfile-jenkins . #build your Jenkins image

4- docker-compose up -d

5- http://your_url:8080 #Jenkins UI

6- http://your_url:3000 #Gitea UI

