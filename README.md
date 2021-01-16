# Docker swarm example for Nestjs

 - simple example of how to deploy nestjs application with postgres on nginx server with help of docker swarm orchestration tool.

## Running the app

 1. First step is to run command:  docker swarm init (This command will initialize swarm mode on machine)
 2. After swarm initialization run docker compose file with command: docker stack deploy --compose-file docker-compose.yml ${stack-name}
