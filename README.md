# UnrealIRCD Docker
[![Docker Pulls](https://img.shields.io/docker/pulls/carterfields/unrealircd?style=for-the-badge)](https://hub.docker.com/r/carterfields/unrealircd)
[![Docker Image Size (tag)](https://img.shields.io/docker/image-size/carterfields/unrealircd/nightly?style=for-the-badge)](https://hub.docker.com/r/carterfields/unrealircd/tags)
[![GitHub](https://img.shields.io/github/license/carterscode/docker-unrealircd?style=for-the-badge)](https://github.com/carterscode/docker-unrealircd)

UnrealIRCd is an Open Source IRC Server, serving thousands of networks since 1999. It runs on Linux, OS X and Windows and is currently the most widely deployed IRCd with a market share of 42%. UnrealIRCd is a highly advanced IRCd with a strong focus on modularity, an advanced and highly configurable configuration file. Key features include SSL/TLS, cloaking, its advanced anti-flood and anti-spam systems, swear filtering and module support. 

# Configuration

The UnnrealIRCd refference config can be found [offical UnrealIRCd reference config](https://raw.githubusercontent.com/unrealircd/unrealircd/unreal50/doc/conf/examples/example.conf) this should be mounted at `/ircd/unrealircd.conf`

# Getting Started

## Docker

HOPM is deployed via docker image like so:

```
docker run -d --name unrealircd \
  -v /path/to/file/hopm.conf:/ircd/unrealircd.conf \
  carterfields/unrealircd:nightly
```

or via docker-compose:

[Official Example](https://raw.githubusercontent.com/carterscode/docker-unrealircd/main/docker-compose.yml)

# Multi-Arch builds

We currently build and publish the following OS/Arch builds of the HOPM container automatically.
* linux/amd64
* linux/arm64
* linux/arm/v7
* linux/arm/v6
* linux/ppc64le
* linux/s390x

# Contributing

All contributions are welcome! Contributing guidelines are in the works
