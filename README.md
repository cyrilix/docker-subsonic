
This repository contains configuration files for building a 
Docker (http://docker.io) image for the Subsonic media streamer.

## Noteworthy

* Subsonic 5.2.1 (http://www.subsonic.org)

## Build your own image

```shell
$ docker build -t <your-name>/docker-subsonic .
```

## Get a pre-built image

A current image is available as a trusted build from the Docker index:

```shell
$ docker pull  cyrilix/docker-subsonic
```

The repository page is at
https://index.docker.io/u/cyrilix/docker-subsonic/


## Run a container with this image

```shell
$ docker run \
  --detach \
  --publish 8080:8080 \
  --volume "/wherever/your/music/is:/opt/music/:ro" \
  <your-name>/subsonic

```
