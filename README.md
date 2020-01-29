# docker-traefik-guide

Example on how you can setup Docker with Traefik.

With this setup you can have e.g. multiple php containers and share the same database container.

# Project directory structure

| Repositories | Docker |
| ------ | ------ |
| projects/traefik | [docker-compose.yml](./traefik/docker-compose.yml) |
| projects/mariadb-phpmyadmin | [docker-compose.yml](./mariadb-phpmyadmin/docker-compose.yml) |
| projects/my-silverstripe-php-application-1 | [docker-compose.yml](./silverstripe-project-1/docker-compose.yml) |

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