# Networking Basics

What it is

Networking basics covers how systems communicate over networks: IP addressing, subnets, routing, and DNS.

Why it is used

Networking is fundamental for connecting components and services in cloud and on-prem systems.

Key concepts

- IP addresses (IPv4/IPv6)
- Subnetting and CIDR notation
- Routing and gateways
- DNS (A, CNAME, TXT, etc.)
- TCP vs UDP
- Ports and firewalls

Commands

- ip addr show
- ip route
- ping 8.8.8.8
- traceroute google.com
- nslookup example.com
- dig example.com

Practical examples

- Calculate subnets for VPC design
- Use dig to verify DNS records
- Trace network path using traceroute

Common interview questions

- Explain CIDR notation and how to split a /24 into /26 networks.
- What is a NAT gateway and when do you use it?
- Differences between routing tables and security groups.

Troubleshooting notes

- Check IP configuration with `ip addr`
- Confirm routes with `ip route`
- Inspect firewall rules (iptables or cloud security groups)

