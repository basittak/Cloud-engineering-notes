# AWS Core Services

What it is

Overview of core AWS services: EC2, S3, IAM, VPC, RDS, Lambda, and CloudFormation.

Why it is used

AWS provides building blocks to run scalable, resilient applications and infrastructure.

Key concepts

- Regions and Availability Zones
- IAM policies and roles
- VPCs, subnets, security groups
- Object storage (S3) vs block storage (EBS)

Commands

- aws s3 ls
- aws ec2 describe-instances
- aws iam get-user

Practical examples

- Upload a file to S3: `aws s3 cp file.txt s3://my-bucket/`
- Launch an EC2 instance with CLI

Common interview questions

- How do security groups differ from network ACLs?
- Explain IAM policies and roles.

Troubleshooting notes

- Check CloudWatch logs
- Ensure IAM permissions for the operation

