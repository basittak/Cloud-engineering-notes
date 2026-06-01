# DNS and Load Balancing

What it is

DNS maps domain names to IP addresses. Load balancers distribute traffic across multiple backend instances to improve availability and scalability.

Why it is used

- DNS provides human-friendly names and failover mechanisms.
- Load balancers ensure high availability and scale traffic.

Key concepts

- DNS records: A, AAAA, CNAME, MX, TXT
- TTL (time to live)
- Types of load balancers: Layer 4 (TCP) vs Layer 7 (HTTP)
- Health checks and session affinity

Commands

- dig example.com A
- nslookup -type=mx example.com

Practical examples

- Configure Route53 A record for a load balancer
- Create an HTTP health check and attach it to a target group

Common interview questions

- How does DNS caching affect propagation?
- Explain the difference between ALB and NLB on AWS.

Troubleshooting notes

- Use dig to verify DNS values and TTLs.
- Check load balancer health checks and logs for failing targets.

