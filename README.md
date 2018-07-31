# [Plex](https://www.plex.tv/) with [docker-compose](https://docs.docker.com/compose/)

This is the skeleton to run your Plex server into your computer.

## How to start

NOTE: You must have `docker` and `docker-compose` installed. Follow official
documentation to install them on your computer.

```
git clone https://github.com/jpahullo/plex-with-docker-compose.git plex
cd plex/docker

```
docker-compose pull

```
Visit https://www.plex.tv/claim to obtain claim token

```
cp .env.example .env

```

replace the PLEX_CLAIM in the above file with the clam from https://www.plex.tv/claim

```
docker-compose up 

```
or

```
docker-compose up -d

```

to daemonize
```

If you do not want to see what's happening behind the scenes, just apply
this last line instead (adding `-d`):

```
docker-compose up -d
```

## Advantages

1. No dependencies on your computer, just docker and docker-compose.
1. Easy installing on every hard disk, even on an external unit.
    * You can have the configuration and all the media on the external hard
      disk, as I do. When you want it to run, just start it with
      `docker-compose up` and let the magics happen.

## Disadvantages

1. You have the docker image of the Plex server still on your computer.

