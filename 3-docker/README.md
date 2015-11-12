# Piwik provisioning with Docker

## Tools used

 - Docker 1.9.0
 - Docker Compose 1.4.1
 - Docker Machine 0.5.0
 - VirtualBox 4.3.26

## Create Development Environment

    cd 3-docker
    docker-machine create --driver virtualbox piwik-docker
    eval "$(docker-machine env piwik-docker)"
    docker-compose build
    docker-compose up -d
