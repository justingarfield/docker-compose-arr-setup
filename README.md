# docker-compose-jollyroger

This repository contains a Docker Compose file that stands-up a rudimentary *arr-based PVR solution backed by Private Internet Access (PIA).

It also overrides the nginx.sh bootstrapping file inside of the docker container, so that reverse proxying can work properly with some of the containers.

## Prerequisties

* Docker Desktop _(or another solution that can provision Docker Compose files)_
* A Private Internet Access (PIA) account

## Usage

### Create your own `.env` file

Copy the `examples/.env` file to the root of the repository and modify it to hold your own values.

### Tailor the volumes in the `docker-compose.yml` file

TODO: Add bit here about adding/removing mapped volumes for media folders in `docker-compose.yml` file

### Pull latest container images

`docker compose pull`

### Start containers and place into background

`docker compose up -d`

### Stop containers and remove them

`docker compose down`
