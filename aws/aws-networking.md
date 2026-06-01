# AWS Networking

What it is

Designing VPCs, subnets, routing, NAT gateways, and VPN/Direct Connect.

Why it is used

To control network isolation, routing, and secure connectivity in AWS.

Key concepts

- VPC CIDR, public vs private subnets
- Internet Gateway vs NAT Gateway
- Route tables and peering

Commands

- aws ec2 describe-vpcs

Practical examples

- Create a VPC with public/private subnets using AWS Console or Terraform

Common interview questions

- Design a multi-AZ VPC for a web application.

Troubleshooting notes

- Confirm route tables and security groups
- Check subnet auto-assign public IP settings

