⚠️ Since [traefik.me doesn't provide keys anymore](https://gist.github.com/pyrou/4f555cd55677331c742742ee6007a73a?permalink_comment_id=5521661#gistcomment-5521661), this project is archived.

# GoldenGateway
Local gateway with Traefik and SSL

## First start

To get SSL certificates, you need to run downloader first.

```sh
docker compose up download-certs
```

## Start

```sh
docker compose up -d
```

## Add services
Make a copy of `docker-compose.override.yaml.dist` into  `docker-compose.override.yaml`. You can add/edit services here.

Each service is accessible as https://{{ serviceName }}.traefik.me or https://{{ serviceName }}-{{ dashedIp }}.traefik.me.

## Traefik Dashboard

Traefik dashboard is available at: https://dashboard.traefik.me/

## Credits
 - [traefik.me](https://traefik.me/) for DNS and SSL
 - Inspiration for docker-compose https://gist.github.com/pyrou/4f555cd55677331c742742ee6007a73a 
