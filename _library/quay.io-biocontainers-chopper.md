---
layout: container
name:  "quay.io/biocontainers/chopper"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/chopper/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/chopper/container.yaml"
updated_at: "2023-03-10 03:25:38.457595"
latest: "0.2.0--hd03093a_0"
container_url: "https://biocontainers.pro/tools/chopper"
aliases:
 - "chopper"
 - "clang"
 - "clang-15"
 - "clang-cl"
 - "clang-cpp"
versions:
 - "0.2.0--hd03093a_0"
description: "singularity registry hpc automated addition for chopper"
config: {"url": "https://biocontainers.pro/tools/chopper", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for chopper", "latest": {"0.2.0--hd03093a_0": "sha256:e790dd0088097b57ec66516905d5113b1a480181ef8359f5df359960d2d7512d"}, "tags": {"0.2.0--hd03093a_0": "sha256:e790dd0088097b57ec66516905d5113b1a480181ef8359f5df359960d2d7512d"}, "docker": "quay.io/biocontainers/chopper", "aliases": {"chopper": "/usr/local/bin/chopper", "clang": "/usr/local/bin/clang", "clang-15": "/usr/local/bin/clang-15", "clang-cl": "/usr/local/bin/clang-cl", "clang-cpp": "/usr/local/bin/clang-cpp"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/chopper.
singularity registry hpc automated addition for chopper
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/chopper
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/chopper:0.2.0--hd03093a_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/chopper/0.2.0--hd03093a_0
$ module help quay.io/biocontainers/chopper/0.2.0--hd03093a_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### chopper-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### chopper-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### chopper-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### chopper-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### chopper-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### chopper-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### chopper

```bash
$ singularity exec <container> /usr/local/bin/chopper
$ podman run --it --rm --entrypoint /usr/local/bin/chopper   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chopper   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### clang

```bash
$ singularity exec <container> /usr/local/bin/clang
$ podman run --it --rm --entrypoint /usr/local/bin/clang   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clang   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### clang-15

```bash
$ singularity exec <container> /usr/local/bin/clang-15
$ podman run --it --rm --entrypoint /usr/local/bin/clang-15   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clang-15   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### clang-cl

```bash
$ singularity exec <container> /usr/local/bin/clang-cl
$ podman run --it --rm --entrypoint /usr/local/bin/clang-cl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clang-cl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### clang-cpp

```bash
$ singularity exec <container> /usr/local/bin/clang-cpp
$ podman run --it --rm --entrypoint /usr/local/bin/clang-cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clang-cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
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