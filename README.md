# docker-traefik-guide

How to setup Docker with Traefik

# Project directory structure

| Repositories | Docker |
| ------ | ------ |
| projects/traefik | docker-compose.yml |
| projects/mysql | docker-compose.yml |
| projects/phpmyadmin | docker-compose.yml |
| projects/my-project-php-application-1 | docker-compose.yml |
| projects/my-project-php-application-2 | docker-compose.yml |

# Installation

## Prerequisites

- Docker
- Docker compose

## Setup

1) Go into each project folder and start up the docker container using the `docker-compose up -d` command.
    ```sh
    $ cd projects/traefik
    $ sudo docker-compose up -d
    ```
2) Visit `localhost:8080/dashboard/` to view the traefik dashboard.