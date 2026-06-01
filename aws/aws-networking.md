# AWS Networking — Concise Notes

Summary

Design and components of AWS VPC networking: CIDR planning, subnets, routing, IGW/NAT, and peering.

Key concepts

- VPC CIDR and subnetting across AZs for HA.
- Public vs private subnets, Internet Gateway (IGW) and NAT Gateway.
- Route tables, NACLs, and security groups.
- VPC peering, Transit Gateway, and Direct Connect.

Commands

- aws ec2 describe-vpcs
- aws ec2 describe-route-tables

Examples

- Typical web-tier: public subnet for ALB, private subnets for app and DB with NAT for outbound updates.

Interview questions

- How would you design a multi-AZ VPC for a three-tier app?
- When to use a NAT Gateway vs NAT instance?

Troubleshooting scenarios

- "No internet from instance": check route table, IGW, and public IP assignment.
- "Cannot reach RDS": verify security groups and subnet group.

Related topics

- Networking basics: ../networking/networking-basics.md
- Terraform AWS networking modules: ../terraform/terraform-aws-pattern.md
