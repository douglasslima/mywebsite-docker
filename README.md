# mywebsite-docker
Building a simple website using docker

Project Structure
.
├── Dockerfile
├── README.md
└── html
    └── index.html

## Setup the docker image

docker build -t mywebsite-docker-image .

list installed images:
docker images -a

## Run the project

docker run --name mywebsie-docker-container -p 80:80 -d mywebsite-docker-image 

## Userful commands
### List running containers
docker ps -a

### Stop the container
docker stop mywebsie-docker-container

### Remove the container
docker rm mywebsie-docker-container




