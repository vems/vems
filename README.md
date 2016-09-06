# VEMS - VEMS Example MicroServices

A monorepo that uses submodules to include the various repos for services, protobufs, and
the api gateway.

This repo also hosts the docs containing the service breakdowns, architecture diagrams,
setup instructions.

(much more to come)

## Quickstart

In order to run this microservice application, be sure to have docker installed. (More
docs will be coming soon to walk through this process, but for now, go
[here](https://docs.docker.com/engine/installation/))

Clone this repo recursivly to include all of the submodule services.

```bash
$ git clone --recursive https://github.com/vems/vems.git
```

`cd` into the directory where it was cloned.

```bash
$ cd vems
```

Build all docker containers required to run this application.

```bash
$ docker-compose build
```

Start all of the docker containers required to run this application.

```bash
$ docker-compose up
```

The application is now running. Visit http://localhost:8080/sum?first=2&second=2 to see
the result of the sum service calculating `2 + 2`.
