## Fiji Dockerfile

This repository contains Dockerfile of [Fiji](fiji.sc) for [janeliascicomp/fiji on DockerHub](https://hub.docker.com/r/janeliascicomp/fiji/).

This is a fork of the official images at [fiji/fiji](https://hub.docker.com/r/fiji/fiji) which:
* Makes the images easier to run with Singularity, e.g. by not setting an internal user
* Let's us release more frequent updates for use in our pipelines

### Base Docker Images

* [openjdk](https://hub.docker.com/_/openjdk)
* [oraclejdk](https://dockerfile.github.io/#/java)

### Docker Tags

`janeliascicomp/fiji` provides multiple tagged images:

* `latest` (default): Fiji with OpenJDK Java 8
* `fiji-openjdk-6`: Fiji with OpenJDK Java 6
* `fiji-openjdk-7`: Fiji with OpenJDK Java 7
* `fiji-openjdk-8`: Fiji with OpenJDK Java 8
* `fiji-oracle-jdk6`: Fiji with Oracle Java 6
* `fiji-oracle-jdk7`: Fiji with Oracle Java 7
* `fiji-oracle-jdk8-arm32v7`: Fiji with Oracle Java 8 for ARM32v7

For example, you can run an *OpenJDK Java 8* container with the following command:

```
  docker run -it --run janeliascicomp/fiji:fiji-openjdk-8
```

### Pre-requisites

* Install [Docker](https://www.docker.com/).
