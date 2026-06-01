# GitHub Collaboration — Concise Notes

Summary

How to use GitHub features: PRs, issues, Actions, branch protection, and code review best practices.

Key concepts

- Pull Requests: review, reviewers, approvals.
- Issues & projects for tracking work.
- GitHub Actions: workflows that run on events.
- Branch protection and required checks.

Practical commands/steps

- Open PR from a feature branch via web UI or `gh` CLI: `gh pr create`.
- Add workflow: `.github/workflows/ci.yml` and monitor Actions tab for runs.

Interview questions

- How do branch protection rules improve code quality?
- What is a required status check?

Troubleshooting scenarios

- "Action failing": open the Actions run, inspect logs, re-run failed jobs.
- "PR cannot merge": check branch protection rules and required checks.

Related topics

- CI/CD pipelines: ../cicd/cicd-basics.md
- Git fundamentals: ../git-github/git-basics.md
