# Kubernetes Basics — Concise Notes

Summary

Core Kubernetes resources and workflows: Pods, Deployments, Services, ConfigMaps, and Secrets.

Key concepts

- Pod: smallest deployable unit; Deployment manages ReplicaSets for scaling.
- Service types: ClusterIP, NodePort, LoadBalancer; Ingress for HTTP routing.
- Namespaces and RBAC for multi-tenant clusters.

Commands

- kubectl get pods
- kubectl apply -f <manifest>
- kubectl describe pod <name>
- kubectl logs <pod>

Examples

- Deploy nginx via Deployment and expose with a ClusterIP Service (see projects/kubernetes-deployment).

Interview questions

- How does Kubernetes scheduling decide where to place Pods?
- What is a ConfigMap vs Secret?

Troubleshooting scenarios

- "CrashLoopBackOff": `kubectl describe pod` and `kubectl logs` to see startup errors.
- "Pod not scheduled": check node resources, taints/tolerations, and events.

Related topics

- K8s networking: ../kubernetes/k8s-networking.md
- Docker images: ../docker/docker-basics.md
