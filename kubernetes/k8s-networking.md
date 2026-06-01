# K8s Networking & Services

What it is

Networking in Kubernetes includes Services, Ingress, and CNI plugins that manage pod-to-pod and external traffic.

Why it is used

To expose services, manage routing, and enforce network policies.

Key concepts

- ClusterIP, NodePort, LoadBalancer
- Ingress controllers and rules
- NetworkPolicies

Commands

- kubectl get svc
- kubectl apply -f ingress.yaml

Practical examples

- Configure an Ingress to route HTTP traffic to multiple services

Common interview questions

- How does service discovery work in Kubernetes?

Troubleshooting notes

- Verify service endpoints and pod labels
- Check ingress controller logs

