---
layout: container
name:  "php"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/php/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/php/container.yaml"
updated_at: "2023-03-10 02:58:41.229690"
latest: "8-alpine3.17"
container_url: "https://hub.docker.com/_/php"
aliases:
 - "php"
 - "php-cgi"
 - "php-config"
 - "phpdbg"
 - "phpize"
versions:
 - "7.3.27-zts-alpine3.12"
 - "8.0.3-alpine"
 - "8.0.5-alpine"
 - "8.0.6-alpine"
 - "8.0.7-alpine"
 - "8.1.0"
 - "8.1.0RC1"
 - "8.1.0alpha1"
 - "8.1.0alpha1-alpine"
 - "8.1.1"
 - "8.1.2"
 - "8.1.3"
 - "latest"
 - "8"
 - "8-alpine3.15"
 - "8.1"
 - "8.0"
 - "7"
 - "8-alpine3.16"
 - "8.2-rc"
 - "8-alpine3.17"
 - "8.2"
description: "While designed for web development, the PHP scripting language also provides general-purpose use."
config: {"docker": "php", "url": "https://hub.docker.com/_/php", "maintainer": "@vsoch", "description": "While designed for web development, the PHP scripting language also provides general-purpose use.", "latest": {"8-alpine3.17": "sha256:8069ceec28b2f5fe4d86e7f66a2183da7f00c4b0aa21bd6e7565a77d5636ae22"}, "tags": {"7.3.27-zts-alpine3.12": "sha256:33c32435b162a6aa427a506f4d3fd3616ab1897a0211c5787649e9e07b967223", "8.0.3-alpine": "sha256:f32cd843417d9271d1500ed3867922175604a243d8033ad1572d617ad7954171", "8.0.5-alpine": "sha256:b728c7e60d1bdb28bfba1bbd4ac3328fbde3a70a959a55c318ccae3fc4d170cf", "8.0.6-alpine": "sha256:a5afa558fcf8030edbc0f160339eaeefccdf1af53df35d0d26171c470a7ab5b6", "8.0.7-alpine": "sha256:edd37734c824c65cdbc1e68c9ac928c590a5c750b6b49c656a302b3b0742d371", "8.1.0": "sha256:b2afd03bcad73aa0a207b0be83310fb2cb35b7a47aceb89e82437b1d19bf81c5", "8.1.0RC1": "sha256:cfa06c39de438a7b7a3977d6412ec580721ad440472b0973ed87ff3758adb0aa", "8.1.0alpha1": "sha256:a63a64bc485982b0543af4ff2fe6e42cd82d65afc39eb4e073f5d361636513fb", "8.1.0alpha1-alpine": "sha256:028c42e86276c77e4bf5d05fb9df93142344d83f971f369a80b6f6e30a50e14b", "8.1.1": "sha256:444ba13f11741642a2692430f6678d47fb028442160ec9a5cfa9da7d3c0a9e07", "8.1.2": "sha256:f1d66b530e99d2e3c2ea302523c5a10ae9e666ddb5ceaacb7dda0af20c7976d7", "8.1.3": "sha256:c0dc322c09db1db4a02f98c97a361a91308c29a3d256703c1e1b64f1ddc28ac6", "latest": "sha256:2f41da28d8f683d4db7cecbbe0cfe2a2ec7ee93ec3de4a7db91d211423fcbaf5", "8": "sha256:2f41da28d8f683d4db7cecbbe0cfe2a2ec7ee93ec3de4a7db91d211423fcbaf5", "8-alpine3.15": "sha256:26d871b044c414dcf3564a018197211627d8b06e7b29415e870a585a2f365c3f", "8.1": "sha256:9d18ffe794c56a6041659270e5eef1bda89ee1e2ec9d1d9a91b43823c73e7777", "8.0": "sha256:082c6f26430ee7598d3adfb77bda9848bfa0ecc9619d5b6a01fb1e62ac5c45f9", "7": "sha256:620a6b9f4d4feef2210026172570465e9d0c1de79766418d3affd09190a7fda5", "8-alpine3.16": "sha256:f1e4987298ec31578a2bb266889524d38a69e73c303b048750c312e43bdd1802", "8.2-rc": "sha256:720733d36d51827f43c1bd6a2eb98482a2f5b7c687f7ad5f8b4919510ca31dbb", "8-alpine3.17": "sha256:8069ceec28b2f5fe4d86e7f66a2183da7f00c4b0aa21bd6e7565a77d5636ae22", "8.2": "sha256:2f41da28d8f683d4db7cecbbe0cfe2a2ec7ee93ec3de4a7db91d211423fcbaf5"}, "aliases": {"php": "/usr/local/bin/php", "php-cgi": "/usr/local/bin/php-cgi", "php-config": "/usr/local/bin/php-config", "phpdbg": "/usr/local/bin/phpdbg", "phpize": "/usr/local/bin/phpize"}}
---

This module is a singularity container wrapper for php.
While designed for web development, the PHP scripting language also provides general-purpose use.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install php
```

Or a specific version:

```bash
$ shpc install php:8-alpine3.17
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load php/8-alpine3.17
$ module help php/8-alpine3.17
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### php-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### php-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### php-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### php-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### php-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### php-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### php

```bash
$ singularity exec <container> /usr/local/bin/php
$ podman run --it --rm --entrypoint /usr/local/bin/php   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/php   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### php-cgi

```bash
$ singularity exec <container> /usr/local/bin/php-cgi
$ podman run --it --rm --entrypoint /usr/local/bin/php-cgi   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/php-cgi   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### php-config

```bash
$ singularity exec <container> /usr/local/bin/php-config
$ podman run --it --rm --entrypoint /usr/local/bin/php-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/php-config   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### phpdbg

```bash
$ singularity exec <container> /usr/local/bin/phpdbg
$ podman run --it --rm --entrypoint /usr/local/bin/phpdbg   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/phpdbg   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### phpize

```bash
$ singularity exec <container> /usr/local/bin/phpize
$ podman run --it --rm --entrypoint /usr/local/bin/phpize   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/phpize   -v ${PWD} -w ${PWD} <container> -c " $@"
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