# Containers

This repository contains the Dockerfiles for the [OpenJDK11](https://pkgs.alpinelinux.org/packages?name=openjdk11&branch=v3.17) images. These images are made available in [Docker Hub](https://hub.docker.com/r/andriimartynov/openjdk/tags).

## Supported Images

In general, we support Alpine linux/amd64 and linux/arm64 containers.

## Build with buildx

```bash
docker buildx create --platform linux/amd64,linux/arm64
loving_roentgen
```

```bash
 docker buildx build --builder loving_roentgen --platform linux/amd64,linux/arm64 --push -t andriimartynov/openjdk:11.0.17-jre .
```