# Python Basics — Concise Notes

Summary

Python essentials: syntax, virtual environments, package management, and common patterns for scripting and apps.

Key concepts

- Data types, functions, modules, and exceptions.
- Virtual envs (`venv`) and dependency files (`requirements.txt`).
- Logging vs print, and packaging basics.

Commands

- python -V
- python -m venv venv
- source venv/bin/activate
- pip install -r requirements.txt

Examples

- Small S3 upload using boto3:

```python
import boto3
s3 = boto3.client('s3')
s3.upload_file('local.txt', 'my-bucket', 'remote.txt')
```

Interview questions

- What is the GIL and when does it matter?
- Differences between lists and generators.

Troubleshooting scenarios

- "ImportError": check virtualenv activation and `pip freeze`.
- "Credential errors": verify AWS credentials environment variables or profile.

Related topics

- Python automation with AWS: ../python/python-automation.md
- Dockerizing Python apps: ../projects/dockerized-application/README_RUN.md
