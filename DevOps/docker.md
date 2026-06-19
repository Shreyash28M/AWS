## What is Docker 
Docker is an open-source containerization platform that allows developers to package applications along with their dependencies into lightweight, portable containers, ensuring consistent execution across different environments.

or 

Docker is an open-source containerization platform that allows developers to package applications along with their dependencies into lightweight, portable containers, ensuring consistent execution across different environments. Containers share the host OS kernel, making them more efficient than virtual machines.

## What is Contair 





## ${\color{lightblue} \textbf{Basic \ Docker \ Commands}}$

### Pull Image from Registry/DockerHub
Downloads a Docker image from the specified registry or DockerHub.
```
1. docker pull <image-name> 

   docker pull <image_name>:<tag>   : pull a specific version image
   example :docker pull ubuntu:22.04

   To pull an image from your own account :
   docker login   : login access the image
   docker pull <username>/<private-repo>:<tag>
   example : docker pull shreyash28m/my-app:v1.0   
```











### Create Container from Image
Creates and starts a container from the specified image.

   ### docker run <image-name> : run docker image(Quick Test Run)
```
   example: docker run hello-world
```
   docker run -d <image-name> : (Detached) Runs the container in the background
   example:docker run -d nginx

   docker run -it <img-name> : Keeps standard input open and allocates a pseudo-terminal for interactive sessions
    example:docker run -it ubuntu bash

   docker run --name <your_custom_name> <image_name>: Assigns a custom name to the container for easier identification.
   example:docker run -d --name my-portfolio nginx

   -v (Volume): Mounts a directory from your host machine into the container to persist or share data.

   -e (Environment): Sets environment variables inside the container using KEY=value format.-

  -rm (Auto-remove): Automatically deletes the container from disk once it stops executing.

3. docker images : to see running docker images 
4. docker ps : to see docker running container
   
   docker ps -a : to see running containers and stopped docker container
   
6. docker stop <container iamge/id> : to stop the running container but even we stopped the container it remain is stopped mode we can restart it later 
7. docker start <image/id> : to start the stopped docker container 
8. docker remove <container iamge/id> : to permanently remove contanier 
9. docker remove -f <container iamge/id> : to  forcefully remove docker container even it's in running  condition
10. 
   docker run -d --rm --name d1 ngnix : it will create a constiner with named d1 and also delete after conatiner is fully created
### remove container if Single Container, Stop the container and then remove it:
   - docker stop <container_id_or_name>
  -  docker rm <container_id_or_name>

    














