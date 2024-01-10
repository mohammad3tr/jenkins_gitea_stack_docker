1-  1- setup your mirror repository:  see https://github.com/mohammad3tr/Docker-Registery.git 

3- docker build -t m3tr-jenkins -f Dockerfile-jenkins . //build your Jenkins image

4-docker-compose up -d

5- http://<your url>:8080 //Jenkins UI

6- http://<your url>:3000 //Gitea UI
