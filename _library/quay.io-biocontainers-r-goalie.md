---
layout: container
name:  "quay.io/biocontainers/r-goalie"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-goalie/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-goalie/container.yaml"
updated_at: "2023-03-09 03:15:46.258310"
latest: "0.6.8--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/r-goalie"

versions:
 - "0.6.0--r41hdfd78af_0"
 - "0.6.6--r42hdfd78af_1"
 - "0.6.7--r42hdfd78af_0"
 - "0.6.8--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for r-goalie"
config: {"url": "https://biocontainers.pro/tools/r-goalie", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-goalie", "latest": {"0.6.8--r42hdfd78af_0": "sha256:de3733dd01c8694d1c72c3cac290438c0267c8b835124ed809190e7ac7b19d1c"}, "tags": {"0.6.0--r41hdfd78af_0": "sha256:a325da85dec2f4b653c6b77314852291f8a6384534a21cc0bab715e4d9581f38", "0.6.6--r42hdfd78af_1": "sha256:b5b8d73740d55553148c7de88b54315d0a5ba843ba468b7fd408f99a72635be2", "0.6.7--r42hdfd78af_0": "sha256:fadea0235c03e420a43588fc7850bde802eb6d0336decf17e909a4a0e6c0f7c7", "0.6.8--r42hdfd78af_0": "sha256:de3733dd01c8694d1c72c3cac290438c0267c8b835124ed809190e7ac7b19d1c"}, "docker": "quay.io/biocontainers/r-goalie"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-goalie.
shpc-registry automated BioContainers addition for r-goalie
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-goalie
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-goalie:0.6.8--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-goalie/0.6.8--r42hdfd78af_0
$ module help quay.io/biocontainers/r-goalie/0.6.8--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-goalie-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-goalie-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-goalie-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-goalie-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-goalie-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-goalie-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-goalie

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
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