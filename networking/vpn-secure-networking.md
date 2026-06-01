# VPN & Secure Networking — Concise Notes

Summary

VPNs and secure networking provide encrypted connectivity between networks or clients and cloud resources.

Key concepts

- VPN types: site-to-site (network-to-network) and client-to-site (remote user).
- Protocols: IPsec (common for site-to-site), OpenVPN, TLS-based tunnels.
- Security controls: network ACLs, security groups, segmentation.

Commands

- `ipsec status` (IPsec tools)
- `openvpn --config client.ovpn` (OpenVPN client)

Examples

- Site-to-site: connect on-prem datacenter to AWS VPC with a VPN gateway.
- SSH tunnel: `ssh -L 8080:internal.host:80 user@jumpbox` to access internal web UI.

Interview questions

- Explain IPsec at a high level.
- When would you use a VPN versus a private managed link (e.g., AWS Direct Connect)?

Troubleshooting scenarios

- "VPN tunnel down": verify shared keys, local/remote IPs, and logs on both endpoints.
- "Latency/packet loss": run `mtr` or `traceroute` and check MTU mismatches.

Related topics

- AWS networking: ../aws/aws-networking.md
- Linux networking tools: ../linux/linux-basics.md
