# Docker Basics

What it is

Docker is a platform for building, shipping, and running containerized applications.

Why it is used

Containers package apps with dependencies for consistent runtime across environments.

Key concepts

- Images vs containers
- Dockerfile and layers
- Registries (Docker Hub, ECR)

Commands

- docker build -t myapp:latest .
- docker run -p 8080:80 myapp:latest
- docker images
- docker ps -a

Practical examples

- Dockerize a simple Python Flask app

Common interview questions

- Explain how Docker images are layered.
- Differences between containers and virtual machines.

Troubleshooting notes

- Check container logs: `docker logs <container>`
- Use `docker inspect` to debug networking and mounts

