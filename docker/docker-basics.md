# Docker Basics — Concise Notes

Summary

Container fundamentals: images, containers, Dockerfile patterns, and registries.

Key concepts

- Images (immutable), layers, tags.
- Containers (runtime instances) and resource limits.
- Dockerfile best practices: small base images, caching, multi-stage builds.

Commands

- docker build -t myapp:latest .
- docker run -p 8080:80 myapp:latest
- docker ps -a
- docker logs <container>

Examples

- Build and run a Flask app (see projects/dockerized-application).

Interview questions

- How do image layers affect build performance?
- Differences between containers and VMs.

Troubleshooting scenarios

- "Container exits immediately": check `docker logs` and `docker inspect` for entrypoint issues.
- "Port not accessible": verify port mapping and host firewall.

Related topics

- Kubernetes deployment: ../kubernetes/kubernetes-basics.md
- Docker Compose: ../docker/docker-compose.md
