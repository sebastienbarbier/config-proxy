This repo manage my personal proxy configuration

# Documentation

## Pre-requirement

- Install [Docker](https://docs.docker.com/engine/install/ubuntu/) and [Docker-compose](https://docs.docker.com/compose/install/) to run init-letsencrypt.sh script.
- Make sure `/var/log/nginx` folder exist.

## Installation

- Pull this repo on server side.
- define MAXMIND_KEY env var
- run install.sh
- run init-letsencrypt.sh