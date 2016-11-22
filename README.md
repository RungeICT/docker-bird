# rungeict/bird
Fedora based image for the BIRD Internet Routing Daemon

[![Docker Repository on Quay](https://quay.io/repository/rungeict/bird/status "Docker Repository on Quay")](https://quay.io/repository/rungeict/bird)

## Introduction
The BIRD project is an attempt to create a routing daemon running on UNIX-like
systems (but not necessarily limited to them) with full support of all modern
routing protocols, easy to use configuration interface and powerful route
filtering language.

http://bird.network.cz/

## Deployment

### Command Line
 ```
 docker run -d --name=bird -p 179:179 --restart=always \
    -v /path/to/bird.conf:/etc/bird.conf rungeict/bird
 ```