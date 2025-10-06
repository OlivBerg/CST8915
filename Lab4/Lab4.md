# Lab 4

[Youtube](https://youtu.be/9-VKSEzFUEU)

## What are the main differences between a Docker image and a Docker container?

A docker image is a read-only template/blueprint that is used to create a container instance. A docker container uses the image to become an instance of that application at runtime.

## Explain how Docker's layered architecture improves efficiency.

The layered architecture significantly improves effeciency through several mechinism:

1. Shared Layers

2. Faster Deployment and Downloads

3. Caching for Faster Builds

4. Immutability and Writable Layer

## Why does each container get its own writable layer?

Because the image is immutable meaning that the core image connot be directly modified. This writable layer allows containers to modify files without affecting the original image.

## What are the benefits of using Docker Compose over running containers individually?

Docker Compose streamlines the devolopment and deployment of an application that utilises several containers by providing a simple way to manage your service. Meaning it basicly runs multiple containers as a single application.
