# Python for Automation

What it is

Using Python scripts and libraries to automate cloud tasks (SDKs, CLI wrappers, APIs).

Why it is used

Automates provisioning, deployments, and operational tasks with readable scripts.

Key concepts

- boto3 (AWS SDK), google-cloud-sdk, azure-sdk
- Idempotence and retries
- Secrets management

Practical examples

- Script to list EC2 instances using boto3

```python
import boto3
ec2 = boto3.client('ec2')
print(ec2.describe_instances())
```

Common interview questions

- How would you retry an API call with exponential backoff in Python?

Troubleshooting notes

- Ensure credentials and environment variables are set
- Use AWS CLI to validate connectivity

