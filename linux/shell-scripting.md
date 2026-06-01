# Shell Scripting — Concise Notes

Summary

Bash scripting for automation: variables, control flow, functions, args, and error handling.

Key concepts

- Shebang, `set -euo pipefail`, and exit codes.
- Positional parameters ($1, $@) and `getopts` for options parsing.
- Functions and returning values.

Commands / Patterns

- Run: `bash script.sh` or `./script.sh` (with +x)
- Debug: `set -x` or run with `bash -x script.sh`

Examples

- Basic backup script:

```bash
#!/usr/bin/env bash
set -euo pipefail
src=$1
dest=$2
tar -czf "$dest" "$src"
```

Interview questions

- How do you safely handle unset variables in bash?
- How would you parse flags like `-f` and `-o`?

Troubleshooting scenarios

- "Script fails silently": add `set -e` and `set -x` to see commands and failures.
- "Subprocess errors swallowed": check exit codes and pipefail behavior.

Related topics

- CI scripts & automation: ../cicd/cicd-basics.md
- Python automation: ../python/python-automation.md
