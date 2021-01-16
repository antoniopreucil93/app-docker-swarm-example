# Docker swarm example for Nestjs

 - Example of how to deploy simple nestjs app, postgres database and nginx server with help of docker swarm orchestration tool.

## Images

 - For building custom nginx image enter into nginx directoy and run following command: docker build -t nginx-server .
 - For building nestjs app image in root direcoty run the following command: docker build -t nest-test .


## Running the app

 1. First step is to run command:  docker swarm init (This command will initialize swarm mode on machine)
 2. After swarm initialization run docker compose file with command: docker stack deploy --compose-file docker-compose.yml ${stack-name}

## Notice

 - If you want to run app with docker compose instead of docker swarm you have to change network from overlay to bridge inside docker-compose file.
