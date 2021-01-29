# Theia IDE

A [Docker](http://docker.com) file to build images for AMD & ARM devices with a installation of [Eclipse Theia IDE](https://theia-ide.org/) an extensible platform to develop multi-language Cloud & Desktop IDEs with state-of-the-art web technologies.

> Be aware! You should read carefully the usage documentation of every tool!

## Thanks to

- [Eclipse Theia IDE](https://theia-ide.org/)

## Details

- [GitHub](https://github.com/DeftWork/theia)
- [Deft.Work my personal blog](http://deft.work)

| Docker Hub | Docker Pulls | Docker Stars | Size/Layers |
| --- | --- | --- | --- |
| [theia](https://hub.docker.com/r/land007/theia-all "land007/theia-all on Docker Hub") | [![](https://img.shields.io/docker/pulls/land007/theia-all.svg)](https://hub.docker.com/r/land007/theia-all "theia on Docker Hub") | [![](https://img.shields.io/docker/stars/land007/theia-all.svg)](https://hub.docker.com/r/land007/theia-all "theia on Docker Hub") | [![](https://images.microbadger.com/badges/image/land007/theia-all.svg)](https://microbadger.com/images/land007/theia-all "theia on microbadger.com") |

## Build Instructions

Build for amd64 arm64 or armv7l architecture (thanks to its [Multi-Arch](https://blog.docker.com/2017/11/multi-arch-all-the-things/) base image)

``` sh
docker build -t land007/theia-all .
```

## Start Theia IDE

``` sh
make start
``` 
Or
``` sh
docker run -d -p 3000:3000 -v "$(pwd):/home/project:cached" land007/theia-all
```
