## What is Docker 
Docker is an open-source containerization platform that allows developers to package applications along with their dependencies into lightweight, portable containers, ensuring consistent execution across different environments.

or 

Docker is an open-source containerization platform that allows developers to package applications along with their dependencies into lightweight, portable containers, ensuring consistent execution across different environments. Containers share the host OS kernel, making them more efficient than virtual machines.

## What is Contair 





## cli 

1. docker pull <image-name> : to take a image from docker registory 
2. docker run -d <img-name> : run a docker image and  create container in detach mode 
3. docker images : to see running docker images 
4. docker ps : to see docker running container
   
   docker ps -a : to see running containers and stopped docker container
   
6. docker stop <container iamge/id> : to stop the running container but even we stopped the container it remain is stopped mode we can restart it later 
7. docker start <image/id> : to start the stopped docker container 
8. docker remove <container iamge/id> : to permanently remove contanier 
9. docker remove -f <container iamge/id> : to  forcefully remove docker container even it's in running  condition
10. 
   docker run -d --rm --name d1 ngnix : it will create a constiner with named d1 and also delete after conatiner is fully created
11. 
