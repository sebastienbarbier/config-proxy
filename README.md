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

## VPN Setup

For VPN functionality, define the following environment variables:

- `VPN_SERVER_URL`: The public URL or IP address of your VPN server (e.g., `vpn.example.com` or `1.2.3.4`)
- `PIHOLE_WEBPASSWORD`: Password for Pi-hole web interface

Then run:
```bash
docker-compose -f docker-compose.vpn.yml up -d
```

## Update proxy conf

- Pull this repo
- User docker command to restart nginx (container name should be config_proxy_nginx)
- run init-letsencrypt.sh

