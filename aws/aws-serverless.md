# AWS Serverless

What it is

Serverless refers to services like AWS Lambda, API Gateway, and managed data stores where you don't manage servers directly.

Why it is used

Lower operational overhead and automatic scaling for event-driven workloads.

Key concepts

- Lambda functions and event sources
- API Gateway + Lambda patterns
- Cold starts and concurrency

Commands

- aws lambda list-functions

Practical examples

- Create a Lambda to process S3 uploads and log events

Common interview questions

- What are cold starts and how to mitigate them?

Troubleshooting notes

- Review CloudWatch logs for function errors
- Check IAM role permissions for the function

