# Kubernetes Basics

What it is

Kubernetes is a container orchestration system for automating deployment, scaling, and management of containerized applications.

Why it is used

To manage complex microservice architectures with declarative APIs.

Key concepts

- Pods, Deployments, Services
- ConfigMaps and Secrets
- Namespaces and RBAC

Commands

- kubectl get pods
- kubectl apply -f deployment.yaml
- kubectl logs <pod>

Practical examples

- Deploy a simple nginx application using a Deployment and Service

Common interview questions

- Describe the Kubernetes control plane components.
- How do rolling updates work in Deployments?

Troubleshooting notes

- Use `kubectl describe` and `kubectl logs` to debug
- Check events and pod status for scheduling issues

