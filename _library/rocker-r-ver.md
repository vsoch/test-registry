---
layout: container
name:  "rocker/r-ver"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/rocker/r-ver/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/rocker/r-ver/container.yaml"
updated_at: "2023-03-09 02:55:36.922207"
latest: "4.2.2"
container_url: "https://hub.docker.com/r/rocker/r-ver"
aliases:
 - "R"
 - "Rscript"
versions:
 - "4.2.2"
 - "3.6.3"
 - "4.1.3"
 - "4.0.5"
description: "Version-stable build of R"
config: {"docker": "rocker/r-ver", "url": "https://hub.docker.com/r/rocker/r-ver", "maintainer": "@marcodelapierre", "description": "Version-stable build of R", "latest": {"4.2.2": "sha256:5e67719080725a6e7ad0f10fe6e42d0cd79df60474e885cc95a57116873e22fb"}, "tags": {"4.2.2": "sha256:5e67719080725a6e7ad0f10fe6e42d0cd79df60474e885cc95a57116873e22fb", "3.6.3": "sha256:9414f76c5f91f24617b5275b8fe4f4ff1313b3b10698a525cac0063c01f2ca6d", "4.1.3": "sha256:99b759d5f41a17ad50d5f2f0c99cb8f51cf78397d196addf538838be1141f03f", "4.0.5": "sha256:2fb770ec2783dcb1ded9eabf34cb74ba3aec85b634151967cc52a40b0e8ce0df"}, "filter": ["^[0-9]+[.][0-9]+[.][0-9]+$"], "aliases": {"R": "/usr/local/bin/R", "Rscript": "/usr/local/bin/Rscript"}}
---

This module is a singularity container wrapper for rocker/r-ver.
Version-stable build of R
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install rocker/r-ver
```

Or a specific version:

```bash
$ shpc install rocker/r-ver:4.2.2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load rocker/r-ver/4.2.2
$ module help rocker/r-ver/4.2.2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-ver-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-ver-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-ver-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-ver-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-ver-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-ver-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### R

```bash
$ singularity exec <container> /usr/local/bin/R
$ podman run --it --rm --entrypoint /usr/local/bin/R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### Rscript

```bash
$ singularity exec <container> /usr/local/bin/Rscript
$ podman run --it --rm --entrypoint /usr/local/bin/Rscript   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Rscript   -v ${PWD} -w ${PWD} <container> -c " $@"
```



In the above, the `<container>` directive will reference an actual container provided
by the module, for the version you have chosen to load. An environment file in the
module folder will also be bound. Note that although a container
might provide custom commands, every container exposes unique exec, shell, run, and
inspect aliases. For anycommands above, you can export:

 - SINGULARITY_OPTS: to define custom options for singularity (e.g., --debug)
 - SINGULARITY_COMMAND_OPTS: to define custom options for the command (e.g., -b)
 - PODMAN_OPTS: to define custom options for podman or docker
 - PODMAN_COMMAND_OPTS: to define custom options for the command

<br>

### Install

You can install shpc locally (for yourself or your user base) as follows:

```bash
$ git clone https://github.com/singularityhub/singularity-hpc
$ cd singularity-hpc
$ pip install -e .
```

Have any questions, or want to request a new module or version? [ask for help!](https://github.com/singularityhub/singularity-hpc/issues)