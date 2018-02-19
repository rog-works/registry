docker-registry
===

# Requirements

* Docker
* docker-compose

# Dependencies

* registry
  * https://docs.docker.com/registry/
* docker-registry-manager
  * https://github.com/snagles/docker-registry-manager

# Usage

## Running registry & Management web server

```bash
$ docker-compose up -d
```

## Access

```bash
$ curl localhost:8080
```

## Tagging

```bash
# usage
$ docker tag <source-container-image:version> <host[:port][/user]/service:version>

# example
$ docker tab hoge:latest localhost:5000/hoge:1.0
```

## Push & Pull

```bash
# push
$ docker push localhost:5000/hoge:1.0

# pull
$ docker pull localhost:5000/hoge:1.0
```
