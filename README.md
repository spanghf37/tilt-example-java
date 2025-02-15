# tilt-example-java

[![Build Status](https://circleci.com/gh/tilt-dev/tilt-example-java/tree/master.svg?style=shield)](https://circleci.com/gh/tilt-dev/tilt-example-java)
[![Contribute](https://img.shields.io/static/v1?label=code%20with&message=che%20(ephemeral)&logo=eclipseche&color=FDB940&labelColor=525C86)](https://che-dogfooding.apps.che-dev.x6e0.p1.openshiftapps.com/#https://github.com/l0rd/tilt-example-java)
[![Contribute](https://img.shields.io/static/v1?label=code%20with&message=che%20(persistent)&logo=eclipseche&color=FDB940&labelColor=525C86)](https://che-dogfooding.apps.che-dev.x6e0.p1.openshiftapps.com/#https://github.com/l0rd/tilt-example-java&df=.devfile-persistent.yaml)

An example project that demonstrates a live-updating Java server in Kubernetes. Read [doc](https://docs.tilt.dev/example_java.html).

We used [Spring Initializr](https://start.spring.io/) to bootstrap the project,
then added Docker & Kubernetes configs for running it in Kubernetes.

To run these examples, you should also have:
- javac (a JDK)
- unzip
- rsync
- python

## Fastest Deployment

This progression of examples shows how to start, and incrementally update
your project for live updates.

- [0-base](0-base): The simplest way to start
- [1-measured](1-measured): Use `local_resource` to measure your deployment time
- [2-optimized](2-optimized): Compile executable Jars and copy them into Docker
- [3-unpacked](3-unpacked): Unpack the executable Jar into Docker layers
- [4-recommended](4-recommended): Live update executable Jars

## Other Configurations

- [101-jib](101-jib): An example of how to integrate Tilt with the [Jib Java
  image builder](https://github.com/GoogleContainerTools/jib)
- [102-jib-live-update](102-jib-live-update): An example of how to use
  live_update with Jib. It requires a lot of knowledge of Jib internals, but you
  can make it work!
- [201-quarkus-live-update](201-quarkus-live-update): An example of how to use
  live_update with [Quarkus](https://quarkus.io/), a container-first, hot-reloading framework for writing
  Java applications.
- [401-spring-boot-layertools](401-spring-boot-layertools): An example of how to
  further optimize the Spring Boot image with the latest recommendations from
  [the Spring Boot Docker
  guide](https://github.com/spring-guides/top-spring-boot-docker#spring-boot-layer-index).

## License

Copyright 2020 tilt.dev

Licensed under [the Apache License, Version 2.0](LICENSE)
