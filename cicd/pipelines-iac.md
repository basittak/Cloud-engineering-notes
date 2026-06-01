# Pipelines and IaC Integration

What it is

Integrating CI/CD pipelines with IaC tools like Terraform to automate infrastructure changes alongside application releases.

Why it is used

To ensure infrastructure changes are reviewed, tested, and applied consistently.

Key concepts

- Pipeline stages (plan, apply)
- Secure handling of secrets and state

Practical examples

- Run `terraform plan` in CI and require manual approval before `apply` in production

Common interview questions

- How do you prevent accidental terraform apply in production from CI?

Troubleshooting notes

- Ensure service account has correct permissions
- Store state remotely and lock during CI runs

