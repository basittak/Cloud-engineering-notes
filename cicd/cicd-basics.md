# CI/CD Basics — Concise Notes

Summary

CI/CD automates building, testing, and deploying applications to deliver changes safely and frequently.

Key concepts

- CI: automated builds and tests on commit.
- CD: automated or gated deployments to environments.
- Environments, artifacts, secrets, and approvals.

Commands / Tools

- GitHub Actions: `.github/workflows/*.yml`
- Common steps: checkout, setup runtime, install dependencies, run tests, build/push image.

Examples

- Simple GitHub Actions workflow: checkout, run tests, build Docker image (see projects/cicd-pipeline).

Interview questions

- Compare blue-green vs canary deployments.
- How would you secure credentials used in pipelines?

Troubleshooting scenarios

- "Pipeline failing": inspect step logs, re-run job, verify environment variables and permissions.
- "Image not pushed": check registry credentials and CI runner network access.

Related topics

- Pipelines + IaC: ../cicd/pipelines-iac.md
- GitHub collaboration: ../git-github/github-collaboration.md
