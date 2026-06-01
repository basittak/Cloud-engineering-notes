# Git Basics — Concise Notes

Summary

Essential Git commands and workflows for collaboration: branching, commits, merges, and recovery.

Key concepts

- Local vs remote, branches, commits, staging area.
- Merge strategies and rebase; pull requests for reviews.
- Recovering with `git reflog`.

Common commands

- git clone <repo>
- git status
- git add .
- git commit -m "msg"
- git checkout -b feature
- git push origin feature
- git pull --rebase

Examples

- Create feature branch, commit changes, push and open a PR:

```
git checkout -b feature/login
git add .
git commit -m "Add login handler"
git push -u origin feature/login
```

Interview questions

- Explain merge vs rebase and when to use each.
- How do you resolve a merge conflict?

Troubleshooting scenarios

- "Detached HEAD": check `git branch` and `git checkout <branch>`.
- "Accidental commit on main": use `git revert` or `git reset` depending on push status.

Related topics

- GitHub Actions CI: ../projects/cicd-pipeline/.github/workflows/ci.yml
- Collaboration on GitHub: ../git-github/github-collaboration.md
