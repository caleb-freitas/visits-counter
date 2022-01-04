# Visits Counter Application

## Docker Compose

- Separated CLI thats installed aling with Docker

- Used to start up multiple Docker containers at the same time

- Automates some of the long-winded arguments passed to `docker-run`

### Some equivalences

`$ docker run <image>` -> `$ docker-compose up`

`$ docker build . && docker run <image>` -> `$ docker-compose up --build`

## Useful commands

Launch in background

`$ docker-compose up -d`

Stop containers

`$ docker-compose down`

## Automatic Container Restarts

### Restart Policies

- no: never attempt to restart this . container if it stops or crashes

- always: if this container stops "for any reason" always attempt to restart it

- on-failure: only restart if the container stops with an error code 

- unless-stopped: always restart unless we (the developers) forcibly stopt it

## Container Status

`$ docker-compose ps`