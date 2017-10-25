# Docker-Webworker
This is just a docker-compose.yml for running [webworker-uploads](https://github.com/kinseyost/webworker-uploads),
[webworker-server](https://github.com/kinseyost/webworker-server), 
[webworker-storage](https://github.com/kinseyost/webworker-storage), and mongodb in docker containers.

## Prerequisites
You must have docker [installed](https://docs.docker.com/engine/installation/)

## Running
1. Create a new directory for running each of the containers in.
2. Copy each of the above directories into that directory
3. Navigate to the webworker-dockerconfig directory and run
```
docker-compose up
```