# VPN and Secure Networking

What it is

VPNs create encrypted tunnels between networks or clients. Secure networking includes encryption, VPNs, and segmentation.

Why it is used

To securely connect remote networks, developers, or microservices and protect data in transit.

Key concepts

- IPsec vs SSL/TLS VPNs
- Site-to-site vs client-to-site VPN
- Subnet isolation and network ACLs
- Encryption in transit

Commands

- ipsec status
- openvpn --config client.ovpn

Practical examples

- Set up a site-to-site VPN between on-prem and AWS
- Use SSH tunnels for secure port forwarding

Common interview questions

- Describe how IPsec works at a high level.
- When should you use a VPN vs a private link?

Troubleshooting notes

- Confirm tunnel endpoints and shared keys
- Inspect VPN logs on both sides

