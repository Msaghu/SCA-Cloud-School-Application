# SCA-Cloud-School-Application
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
