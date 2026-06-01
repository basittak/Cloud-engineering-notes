# Terraform Basics — Concise Notes

Summary

Terraform basics: declarative IaC, providers, resources, state, and modules.

Key concepts

- .tf files declare resources; `terraform plan` previews changes.
- State file stores current infra mapping; backends (S3 + DynamoDB) recommended.
- Modules encapsulate reusable configurations.

Commands

- terraform init
- terraform fmt
- terraform plan
- terraform apply
- terraform destroy

Examples

- Create an S3 bucket resource and output its name (see projects/terraform-aws-infrastructure).

Interview questions

- Why store remote state and how do you lock it?
- What are Terraform modules and when to use them?

Troubleshooting scenarios

- "State drift": run `terraform plan` to detect differences and reconcile carefully.
- "Provider version conflicts": pin provider versions in `required_providers`.

Related topics

- AWS infra via Terraform: ../projects/terraform-aws-infrastructure/README.md
- CI integration: ../cicd/pipelines-iac.md
