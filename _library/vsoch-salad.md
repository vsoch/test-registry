---
layout: container
name:  "vsoch/salad"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/vsoch/salad/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/vsoch/salad/container.yaml"
updated_at: "2023-03-08 18:38:36.209268"
latest: "latest"
container_url: "https://singularity-hpc.readthedocs.io"

versions:
 - "latest"
description: "A custom container to do X."
config: {"url": "https://singularity-hpc.readthedocs.io", "maintainer": "Dinosaur", "description": "A custom container to do X.", "latest": {"latest": "crane digest vsoch/salad:latest: UNAUTHORIZED: authentication required; [map[Action:pull Class: Name:vsoch/salad Type:repository]]"}, "tags": {"latest": "crane digest vsoch/salad:latest: UNAUTHORIZED: authentication required; [map[Action:pull Class: Name:vsoch/salad Type:repository]]"}, "docker": "vsoch/salad"}
---

This module is a singularity container wrapper for vsoch/salad.
A custom container to do X.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install vsoch/salad
```

Or a specific version:

```bash
$ shpc install vsoch/salad:latest
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load vsoch/salad/latest
$ module help vsoch/salad/latest
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### salad-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### salad-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### salad-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### salad-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### salad-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### salad-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### salad

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