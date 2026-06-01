# Kubernetes Networking & Services — Concise Notes

Summary

Services, Ingress, and CNI control pod connectivity and external exposure in Kubernetes.

Key concepts

- Types of Services: ClusterIP (internal), NodePort (port on nodes), LoadBalancer (cloud LB).
- Ingress and IngressController (Nginx, Traefik) for HTTP routing and TLS termination.
- NetworkPolicy for enforcing pod-level networking rules.

Commands

- kubectl get svc, kubectl get ingress
- kubectl apply -f ingress.yaml

Examples

- Configure an Ingress rule to route /api to service-a and /web to service-b.

Interview questions

- How does a Service discover backend pods?
- When would you use NetworkPolicy?

Troubleshooting scenarios

- "Ingress 404": check ingress rules, service selectors, and ingress controller logs.
- "Cross-namespace communication failing": inspect NetworkPolicies and service references.

Related topics

- Kubernetes basics: ../kubernetes/kubernetes-basics.md
- Cloud load balancers: ../networking/dns-load-balancing.md
