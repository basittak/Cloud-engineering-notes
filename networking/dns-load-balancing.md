# DNS & Load Balancing — Concise Notes

Summary

How DNS maps names to addresses and how load balancers distribute traffic to improve availability and scale.

Key concepts

- DNS record types: A, AAAA, CNAME, TXT, MX; TTL controls caching.
- Load balancer layers: L4 (TCP) vs L7 (HTTP/HTTPS).
- Health checks, sticky sessions, target groups.
- CDN vs Load Balancer: CDN caches content geographically; LB distributes live traffic.

Commands

- dig example.com A
- nslookup -type=mx example.com

Examples

- Route53: create A record pointing to an ALB.
- CloudFront + S3: use DNS to map custom domain to CloudFront distribution.

Interview questions

- When would you use a CNAME vs an A record?
- Explain differences between an ALB and an NLB (AWS).

Troubleshooting scenarios

- "DNS not updated": check TTL, DNS provider console, and `dig` from multiple resolvers.
- "Unhealthy targets": inspect load balancer health checks and backend logs.

Related topics

- AWS core services: ../aws/aws-core-services.md
- Kubernetes Ingress: ../kubernetes/k8s-networking.md
