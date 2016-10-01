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