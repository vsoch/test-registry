---
layout: container
name:  "quay.io/biocontainers/sage-proteomics"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/sage-proteomics/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/sage-proteomics/container.yaml"
updated_at: "2023-03-10 03:38:46.402176"
latest: "0.8.1--hec16e2b_0"
container_url: "https://biocontainers.pro/tools/sage-proteomics"
aliases:
 - "sage"
versions:
 - "0.8.1--hec16e2b_0"
description: "singularity registry hpc automated addition for sage-proteomics"
config: {"url": "https://biocontainers.pro/tools/sage-proteomics", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for sage-proteomics", "latest": {"0.8.1--hec16e2b_0": "sha256:c66ead864888868623284914f811e4c4c2894a8bb7bb6d55f55bb5aae15dcf6f"}, "tags": {"0.8.1--hec16e2b_0": "sha256:c66ead864888868623284914f811e4c4c2894a8bb7bb6d55f55bb5aae15dcf6f"}, "docker": "quay.io/biocontainers/sage-proteomics", "aliases": {"sage": "/usr/local/bin/sage"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/sage-proteomics.
singularity registry hpc automated addition for sage-proteomics
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/sage-proteomics
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/sage-proteomics:0.8.1--hec16e2b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/sage-proteomics/0.8.1--hec16e2b_0
$ module help quay.io/biocontainers/sage-proteomics/0.8.1--hec16e2b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### sage-proteomics-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### sage-proteomics-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### sage-proteomics-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### sage-proteomics-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### sage-proteomics-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### sage-proteomics-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### sage

```bash
$ singularity exec <container> /usr/local/bin/sage
$ podman run --it --rm --entrypoint /usr/local/bin/sage   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sage   -v ${PWD} -w ${PWD} <container> -c " $@"
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