# Basic Docker Commands Tutorial

This tutorial covers the fundamental commands in Docker, a powerful tool for developing, shipping, and running applications in isolated environments called containers.

## Getting Started

### 1. Installing Docker

Before you begin, ensure Docker is installed on your system. Installation guides for various platforms are available at the official Docker website.

## Docker Command Basics

### 2. Docker Version

```bash
docker --version
```
- Checks the installed Docker version.

### 3. Running a Container

```bash
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```
- Runs a Docker container from an image.
- Common options:
  - `-d`: Runs container in detached mode (in the background).
  - `-p`: Maps a port from the container to the host.
  - `--name`: Assigns a name to the container.

### 4. Listing Containers

```bash
docker ps [OPTIONS]
```
- Lists running containers.
- Common options:
  - `-a`: Shows all containers (default shows just running).

### 5. Stopping a Container

```bash
docker stop [OPTIONS] CONTAINER [CONTAINER...]
```
- Stops one or more running containers.

### 6. Starting a Stopped Container

```bash
docker start [OPTIONS] CONTAINER [CONTAINER...]
```
- Starts one or more stopped containers.

### 7. Removing a Container

```bash
docker rm [OPTIONS] CONTAINER [CONTAINER...]
```
- Removes one or more containers.
- Use `-f` to force removal of a running container.

## Working with Images

### 8. Pulling an Image

```bash
docker pull [OPTIONS] NAME[:TAG|@DIGEST]
```
- Pulls an image from a registry (like Docker Hub).

### 9. Listing Images

```bash
docker images [OPTIONS] [REPOSITORY[:TAG]]
```
- Lists images present on the local system.

### 10. Removing an Image

```bash
docker rmi [OPTIONS] IMAGE [IMAGE...]
```
- Removes one or more images.

## Dockerfile and Building Images

### 11. Building an Image

```bash
docker build [OPTIONS] PATH | URL | -
```
- Builds an image from a Dockerfile.
- Common options:
  - `-t`: Tags the image with a name.

## Docker Compose

Docker Compose is used to define and run multi-container Docker applications.

### 12. Running Docker Compose

```bash
docker-compose up [OPTIONS]
```
- Builds, (re)creates, starts, and attaches to containers for a service.

### 13. Stopping Docker Compose

```bash
docker-compose down [OPTIONS]
```
- Stops and removes containers, networks, volumes, and images created by `up`.

## Additional Commands

### 14. Viewing Logs

```bash
docker logs [OPTIONS] CONTAINER
```
- Fetches the logs of a container.

### 15. Executing Commands in a Container

```bash
docker exec [OPTIONS] CONTAINER COMMAND [ARG...]
```
- Executes a command in a running container.

---

*Note: This is a basic guide and covers only the most commonly used Docker commands. For a comprehensive list and detailed explanations, refer to the [Docker Documentation]([https://docs.docker.com/](https://docs.docker.com/get-started/overview/)https://docs.docker.com/get-started/overview/).*
```
