---
layout: container
name:  "quay.io/biocontainers/iqtree"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/iqtree/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/iqtree/container.yaml"
updated_at: "2023-03-09 03:22:35.130476"
latest: "2.2.0.3--hb97b32f_1"
container_url: "https://biocontainers.pro/tools/iqtree"
aliases:
 - "iqtree"
 - "iqtree2"
versions:
 - "2.2.0_beta--hb97b32f_1"
 - "2.2.0.3--hb97b32f_1"
description: "shpc-registry automated BioContainers addition for iqtree"
config: {"url": "https://biocontainers.pro/tools/iqtree", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for iqtree", "latest": {"2.2.0.3--hb97b32f_1": "sha256:a4d3f266bfac25f8018eaf03b14db48c66aa6eb02391ad28cf19520d61c3e5fb"}, "tags": {"2.2.0_beta--hb97b32f_1": "sha256:96ca289717c1d1d07536802939f2da66c22ccf7e527b22297c78de585358e1c3", "2.2.0.3--hb97b32f_1": "sha256:a4d3f266bfac25f8018eaf03b14db48c66aa6eb02391ad28cf19520d61c3e5fb"}, "docker": "quay.io/biocontainers/iqtree", "aliases": {"iqtree": "/usr/local/bin/iqtree", "iqtree2": "/usr/local/bin/iqtree2"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/iqtree.
shpc-registry automated BioContainers addition for iqtree
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/iqtree
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/iqtree:2.2.0.3--hb97b32f_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/iqtree/2.2.0.3--hb97b32f_1
$ module help quay.io/biocontainers/iqtree/2.2.0.3--hb97b32f_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### iqtree-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### iqtree-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### iqtree-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### iqtree-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### iqtree-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### iqtree-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### iqtree

```bash
$ singularity exec <container> /usr/local/bin/iqtree
$ podman run --it --rm --entrypoint /usr/local/bin/iqtree   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/iqtree   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### iqtree2

```bash
$ singularity exec <container> /usr/local/bin/iqtree2
$ podman run --it --rm --entrypoint /usr/local/bin/iqtree2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/iqtree2   -v ${PWD} -w ${PWD} <container> -c " $@"
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