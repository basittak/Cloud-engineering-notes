# Networking Basics — Concise Notes

Summary

Essential networking concepts for cloud engineers: IP addressing, subnets, routing, DNS, and transport protocols.

Key concepts

- IP addressing & CIDR: IPv4/IPv6, CIDR notation (e.g., 10.0.0.0/16).
- Subnetting: dividing CIDR blocks into smaller networks for isolation.
- Routing: route tables, default gateways, and static vs dynamic routing.
- DNS: name resolution (A, CNAME, TXT), TTL, propagation.
- Transport: TCP (reliable) vs UDP (connectionless).
- Firewalls & security groups: permit/deny by port and protocol.

Commands (practice)

- ip addr show
- ip route show
- ping 8.8.8.8
- traceroute example.com
- dig example.com +short
- nslookup example.com

Examples

- Calculate subnets: split 10.0.0.0/24 into four /26 networks.
- Verify DNS: `dig +short www.example.com`.
- Trace path: `traceroute github.com`.

Interview questions

- Explain CIDR and how to split a network.
- What is the difference between TCP and UDP?
- How does DNS caching affect record changes?

Troubleshooting scenarios

- "No network access": check `ip addr`, `ip route`, and firewall rules.
- "Can't resolve hostname": run `dig`/`nslookup`, verify DNS servers and /etc/resolv.conf.
- "Packets dropped": use `traceroute` to find the failing hop.

Related topics

- VPC & AWS networking: ../aws/aws-networking.md
- Kubernetes networking: ../kubernetes/k8s-networking.md
- Security groups & Linux firewall: ../linux/linux-basics.md
