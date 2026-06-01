# Docker Compose — Concise Notes

Summary

Compose manages multi-container apps via a YAML file describing services, networks, and volumes.

Key concepts

- service definitions, dependency order, named volumes, and networks.
- `docker-compose up` vs `docker-compose up --build`.

Commands

- docker-compose up -d
- docker-compose logs -f
- docker-compose down --volumes

Examples

- Compose a web app + Postgres service for local development.

Interview questions

- How do you persist data between container restarts?
- How to scale a service with Docker Compose?

Troubleshooting scenarios

- "Service can't connect to DB": check network aliases and environment variables in compose file.
- "Volume permissions": adjust UID/GID or use `volumes: :cached` options.

Related topics

- Local dev to Kubernetes: ../projects/kubernetes-deployment/README.md
