# Docker

Docker is an enclosed environment for applications, so that you do not need to consider what OS you are using or make your own virtual environments.

Docker itself a Linux Container, which is a type of virtual environment, but lighter than making an entire VM for any given project.

## Images and Containers

An image is a snapshot of a project

A container is a running instance of a project

### Layers

All images are comprised of a series of layers, the base layer is usually the linux version chosen.

## Dockerfile

Similar to a requirements.txt or pyproject.toml, a Dockerfile will have the data for a docker project.

Docker files are read from top to bottom, and the fist line *MUST* be the `FROM` command:

```Docker
FROM python:3.7-alpine
```

[<-- Back](../README.md)
