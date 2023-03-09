---
layout: container
name:  "quay.io/biocontainers/r-misha"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-misha/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-misha/container.yaml"
updated_at: "2023-03-09 03:06:22.769393"
latest: "4.1.0--r42h87f3376_4"
container_url: "https://biocontainers.pro/tools/r-misha"

versions:
 - "4.1.0--r41h87f3376_3"
 - "4.1.0--r42h87f3376_4"
description: "shpc-registry automated BioContainers addition for r-misha"
config: {"url": "https://biocontainers.pro/tools/r-misha", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-misha", "latest": {"4.1.0--r42h87f3376_4": "sha256:a5d293d63c1b36194cb09436337fb9700e4112b62169bb5da5074645b552f8bc"}, "tags": {"4.1.0--r41h87f3376_3": "sha256:2e6e7f9883bf497da9b96c25564dd1976f53f2ec3d4570226e36c5d7d9af2b27", "4.1.0--r42h87f3376_4": "sha256:a5d293d63c1b36194cb09436337fb9700e4112b62169bb5da5074645b552f8bc"}, "docker": "quay.io/biocontainers/r-misha"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-misha.
shpc-registry automated BioContainers addition for r-misha
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-misha
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-misha:4.1.0--r42h87f3376_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-misha/4.1.0--r42h87f3376_4
$ module help quay.io/biocontainers/r-misha/4.1.0--r42h87f3376_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-misha-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-misha-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-misha-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-misha-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-misha-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-misha-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-misha

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