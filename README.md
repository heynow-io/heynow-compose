# heynow-compose
Docker-Compose script for Heynow.io

## Requirements

- Docker (or Docker Machine if you're on Windows/Mac)
- Docker Compose (it's already preinstalled with docker toolbox)
- Having access to all required images; At the time of writing these would be:
    - io.heynow.eureka
    - io.heynow.configserver
    - io.heynow.heynow-edge

## Usage
Execute the following command in your terminal:
```
docker-compose up
```

As the intertwined logs may get quire messy you may also use this command to run all the containers in detached mode:
```
docker-compose up -d
```

## Setting up 

From clear server:
    - curl -L "https://github.com/docker/compose/releases/download/1.8.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    - chmod +x /usr/local/bin/docker-compose
    - curl https://get.docker.com | sh
    - systemctl start docker
