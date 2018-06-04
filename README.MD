# Docker-Webworker
This is just a docker-compose.yml for running [webworker-uploads](https://github.com/kinseyost/webworker-uploads),
[webworker-server](https://github.com/kinseyost/webworker-server), 
[webworker-storage](https://github.com/kinseyost/webworker-storage), and mongodb in docker containers.

## Prerequisites
You must have docker [installed](https://docs.docker.com/engine/installation/)

## Running
1. Create a new directory for running each of the containers in.
```
mkdir ~/http-proxy-poc
cd ~/http-proxy-poc
```
2. Copy each of the above directories into that directory
```
git clone https://github.com/kinseyost/webworker-uploads.git
```
```
git clone https://github.com/kinseyost/webworker-server.git
```
```
git clone https://github.com/kinseyost/webworker-storage.git
```
```
git clone https://github.com/kinseyost/webworker-dockerconfig.git
```
3. Navigate to the webworker-dockerconfig directory and run `docker-compose up`
```
cd webworker-dockerconfig
docker-compose up
```

Docker will pull/build all of the necessary images
Once this completes, you will be able to navigate to 
[http://localhost:3000](http://localhost:3000)

**Note**: If you have mongodb running in any other docker containers, you may have conflicts.  Make sure this to stop any conflicting services.