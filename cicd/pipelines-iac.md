# Pipelines & IaC Integration — Concise Notes

Summary

How to safely run infrastructure IaC (Terraform) inside CI pipelines with plan/apply separation and approvals.

Key concepts

- Pipeline stages: plan (preview), review/approval, apply (execution).
- Remote state locking and secure credentials for CI.
- Use ephemeral service accounts with limited permissions.

Commands / Patterns

- Run `terraform plan -out=tfplan && terraform show -json tfplan` in CI
- Require manual approval before `terraform apply tfplan` on prod.

Interview questions

- How do you prevent accidental infra changes via CI?
- How do you test Terraform code before applying to prod?

Troubleshooting scenarios

- "State locked by another run": inspect locks in the backend (DynamoDB) and running jobs.
- "CI apply failed": ensure the CI role has required permissions and environment variables.

Related topics

- Terraform remote state: ../terraform/terraform-aws-pattern.md
- CI/CD workflows: ../projects/cicd-pipeline/README.md
