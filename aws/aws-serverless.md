# AWS Serverless — Concise Notes

Summary

Serverless services like Lambda and API Gateway let you run code without managing servers; good for event-driven workloads.

Key concepts

- Lambda function model: handler, runtime, IAM execution role.
- Triggers: S3 events, API Gateway, SNS, SQS.
- Cold starts and ways to mitigate (provisioned concurrency).

Commands

- aws lambda list-functions
- aws logs tail /aws/lambda/<fn-name> --follow

Examples

- S3 -> Lambda: process file uploads and write metadata to DynamoDB.

Interview questions

- What causes cold starts and how to reduce them?
- How do you secure an API Gateway-backed Lambda?

Troubleshooting scenarios

- "Function error": inspect CloudWatch logs and check IAM role permissions.
- "Timeouts": increase function timeout or optimize code and dependencies.

Related topics

- IAM roles & policies: ../aws/aws-core-services.md
- CI/CD for serverless: ../cicd/pipelines-iac.md
