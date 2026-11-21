# Hello Captain - Docker Project

A beginner Docker project demonstrating how to build a Docker image using Alpine Linux and pass custom build arguments.

## Technologies Used
- Docker
- Alpine Linux
- Dockerfile

## Docker Concepts Practiced
- FROM
- ARG
- ENV
- CMD
- Docker Image Building
- Docker Container Execution

## Build the Image

```bash
docker build --build-arg NAME=Dilak -t hello-captain:v1 .
```

## Run the Container

```bash
docker run --rm hello-captain:v1
```

Expected output:

```text
Hello, Dilak!
```

## Run with a Different Name

```bash
docker run --rm -e NAME=John hello-captain:v1
```

Expected output:

```text
Hello, John!
```

## Learning Outcome

Understanding the difference between Docker build-time arguments (ARG) and runtime environment variables (ENV), and how CMD executes commands when a container starts.