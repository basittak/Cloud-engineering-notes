# Python for Automation — Concise Notes

Summary

Using Python SDKs to automate cloud tasks (e.g., boto3 for AWS) with idempotence and retries.

Key concepts

- SDK clients (boto3 clients/resources), sessions and profiles.
- Idempotence, exponential backoff, error handling.
- Secrets handling (environment vars, secrets manager).

Commands / Snippets

- `aws configure` to set up CLI; Python uses same credentials.

Example: list EC2 instances

```python
import boto3
ec2 = boto3.client('ec2')
print(ec2.describe_instances())
```

Interview questions

- How would you implement retries with exponential backoff?
- How to securely store API keys for automation?

Troubleshooting scenarios

- "AccessDenied": verify IAM role/credentials and region.
- "Throttling": implement retries and exponential backoff.

Related topics

- Terraform automation: ../terraform/terraform-basics.md
- CI scripts: ../cicd/pipelines-iac.md
