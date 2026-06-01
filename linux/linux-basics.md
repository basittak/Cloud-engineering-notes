# Linux Basics

What it is

Linux basics include the command line, file system, users, permissions, and basic administration.

Why it is used

Most cloud servers and container base images run Linux. Understanding it is essential for debugging and automation.

Key concepts

- Filesystem layout (/etc, /var, /home, /opt)
- Users and groups
- Permissions (rwx, chmod, chown)
- Processes and signals
- Package management (apt, yum)

Commands

- ls, cd, pwd
- cat, less, tail -f
- ps aux, top, htop
- systemctl status nginx
- chmod 644 file.txt
- chown user:group file.txt

Practical examples

- SSH into a server and inspect logs in /var/log
- Use `systemctl` to manage services

Common interview questions

- How do file permissions work? Explain u/g/o and rwx.
- How would you find a process consuming high CPU?

Troubleshooting notes

- Check disk usage with `df -h` and `du -sh`
- Review logs in /var/log for service errors

