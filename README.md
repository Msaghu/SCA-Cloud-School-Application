# SCA-Cloud-School-Application

What is Docker?

What is a Dockerfile?

What is a Docker container?

What is a Docker image?

Installing Docker on local machine:
`docker`

To check the docker version, run
`docker version`
It will give the following output
```
Client:
 Cloud integration: v1.0.35+desktop.5
 Version:           24.0.7
 API version:       1.43
 Go version:        go1.20.10
 Git commit:        afdd53b
 Built:             Thu Oct 26 09:08:44 2023
 OS/Arch:           windows/amd64
 Context:           default

Server: Docker Desktop 4.26.1 (131620)
 Engine:
  Version:          24.0.7
  API version:      1.43 (minimum version 1.12)
  Go version:       go1.20.10
  Git commit:       311b9ff
  Built:            Thu Oct 26 09:08:02 2023
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          1.6.25
  GitCommit:        d8f198a4ed8892c764191ef7b3b06d8a2eeb5c7f
 runc:
  Version:          1.1.10
  GitCommit:        v1.1.10-0-g18a0cb0
 docker-init:
  Version:          0.19.0
  GitCommit:        de40ad0
```

Common commands:

1. `docker pull`
2. `docker run`
3. `docker ps`
4. `docker images`

A Dockerfile that displays a web page
Deploying a static website as a container
1. create a directory - shecodeafrica
2. Change into the directory
3. create a html file using the VIM editor displaying the message "Welcome to SCA Cloud School Application"
4. Create a Dockerfile showing:
from the NGINX server (choosethe smallest, i chose alpine)
copy from the static directory where the static files are stored
5. Build the docker image 
6. View that the docker image has been created, and you can filter through the command : sudo docker images ¦ grep shecodeafrica
7. Run the docker image and name the container in the command
(-d flag is to run the daemon in the backround, --name to name the container)
sudo docker run -d --name shecodeafricaapp-container -p 80:80 shecodeafrica-app:v1
8. View the running processes using sudo docker ps
9. viewing on localshost shows the message "Welcome to SCA Cloud School Application"
10. View logs using : 
