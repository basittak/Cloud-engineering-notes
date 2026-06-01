# AWS Core Services — Concise Notes

Summary

High-level overview of key AWS services used by cloud engineers: EC2, S3, IAM, VPC, RDS, Lambda.

Key concepts

- Regions & AZs for fault isolation and latency.
- IAM: users, groups, roles, and least-privilege.
- Compute: EC2 instances, instance types, EBS volumes.
- Storage: S3 objects (eventual/strong consistency depending on ops), lifecycle rules.
- Networking: VPC, subnets, IGW, NAT, security groups.
- Serverless: Lambda, API Gateway, and event-driven patterns.

Commands

- aws s3 ls
- aws ec2 describe-instances
- aws iam get-user

Examples

- Upload file: `aws s3 cp file.txt s3://my-bucket/`
- Start instance (CLI): `aws ec2 run-instances --image-id ami-... --count 1 --instance-type t3.micro`

Interview questions

- Explain security groups vs network ACLs.
- How does S3 durability and availability work?

Troubleshooting scenarios

- "Permissions error": verify IAM policy and role used by the caller.
- "Instance unreachable": check security groups, route tables, and public IP assignment.

Related topics

- VPC design: ../aws/aws-networking.md
- Serverless patterns: ../aws/aws-serverless.md
