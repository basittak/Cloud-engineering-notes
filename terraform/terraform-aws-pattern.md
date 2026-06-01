# Terraform AWS Pattern

What it is

Best practices for using Terraform with AWS including module structure, remote state, and IAM permissions.

Why it is used

To scale IaC, enforce patterns, and enable team collaboration safely.

Key concepts

- Remote state (S3 + DynamoDB locking)
- Module composition and registry
- Least-privilege IAM for automation

Practical examples

- Example backend configuration to store state in S3

Common interview questions

- How do you handle secrets in Terraform?

Troubleshooting notes

- Check provider versions and `terraform init` results
- Monitor state locking errors

