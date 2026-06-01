# Terraform AWS Patterns — Concise Notes

Summary

Best practices for Terraform on AWS: remote state, modules, naming, and least-privilege IAM.

Key concepts

- Remote backend: S3 bucket with DynamoDB for state locking.
- Workspaces vs per-environment state files.
- IAM permissions for automation (CI) are tightly scoped.

Commands / Snippets

- Backend example in `backend.tf`:

```
terraform {
  backend "s3" {
    bucket = "tf-state-bucket"
    key    = "envs/prod/terraform.tfstate"
    region = "us-east-1"
  }
}
```

Interview questions

- How do you manage secrets in Terraform?
- How to perform safe rollouts of infra changes?

Troubleshooting scenarios

- "State lock present": check DynamoDB table and running CI jobs; manually unlock only when safe.
- "Apply fails due to permissions": verify IAM role used by CI has required actions.

Related topics

- Terraform basics: ../terraform/terraform-basics.md
- AWS networking: ../aws/aws-networking.md
