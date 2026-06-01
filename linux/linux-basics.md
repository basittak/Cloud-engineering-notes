# Linux Basics — Concise Notes

Summary

Core Linux skills for cloud engineers: filesystem, users/permissions, processes, package management, and service control.

Key concepts

- Filesystem layout (/, /etc, /var, /home).
- Users & groups; permissions (rwx) and ownership.
- Processes and systemd: units, `systemctl`.
- Logs in /var/log and journalctl.

Commands

- ls, cd, pwd
- cat / tail / less: `tail -f /var/log/syslog`
- ps aux, top, htop
- systemctl status <service>
- df -h, du -sh <path>
- chmod/chown: `chmod 644 file`, `chown user:group file`

Examples

- Check disk: `df -h`; find large folders: `du -sh /var/* | sort -h`.
- Restart a service: `sudo systemctl restart nginx` and view logs: `journalctl -u nginx -f`.

Interview questions

- Explain Linux file permissions and how to set them.
- How do you find which process is using a port?

Troubleshooting scenarios

- "Service won't start": check `systemctl status` and logs in `/var/log`.
- "Disk full": identify large files with `du` and clear rotated logs.

Related topics

- Shell scripting: ../linux/shell-scripting.md
- Containers & Docker base images: ../docker/docker-basics.md
