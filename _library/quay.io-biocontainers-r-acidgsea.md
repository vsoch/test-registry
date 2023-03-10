---
layout: container
name:  "quay.io/biocontainers/r-acidgsea"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-acidgsea/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-acidgsea/container.yaml"
updated_at: "2023-03-10 03:42:50.823953"
latest: "0.8.7--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/r-acidgsea"
aliases:
 - "pandoc"
versions:
 - "0.7.0--r41hdfd78af_0"
 - "0.8.6--r42hdfd78af_1"
 - "0.7.0--r41hdfd78af_1"
 - "0.8.7--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for r-acidgsea"
config: {"url": "https://biocontainers.pro/tools/r-acidgsea", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-acidgsea", "latest": {"0.8.7--r42hdfd78af_0": "sha256:dca58f664ebb2a024edd13be02639ba7c54523aacc43a86cda90137c22ca9737"}, "tags": {"0.7.0--r41hdfd78af_0": "sha256:d7f1697ab2efbaeea41765f2fed52efdcc30046c9c7519d55e96877792bc2ddc", "0.8.6--r42hdfd78af_1": "sha256:a744b6b624d8993b6cd75b776a6c27a209fd718337466aa132f2c40be40c3eca", "0.7.0--r41hdfd78af_1": "sha256:9e39dc0dae3468d2291bc5c468df93d7daadf3fc24496f52ddcd025ef78e749e", "0.8.7--r42hdfd78af_0": "sha256:dca58f664ebb2a024edd13be02639ba7c54523aacc43a86cda90137c22ca9737"}, "docker": "quay.io/biocontainers/r-acidgsea", "aliases": {"pandoc": "/usr/local/bin/pandoc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-acidgsea.
shpc-registry automated BioContainers addition for r-acidgsea
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-acidgsea
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-acidgsea:0.8.7--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-acidgsea/0.8.7--r42hdfd78af_0
$ module help quay.io/biocontainers/r-acidgsea/0.8.7--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-acidgsea-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-acidgsea-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-acidgsea-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-acidgsea-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-acidgsea-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-acidgsea-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pandoc

```bash
$ singularity exec <container> /usr/local/bin/pandoc
$ podman run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
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