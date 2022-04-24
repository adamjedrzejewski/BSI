# Failed SSH login attempts analysis

1. `ssh <user>@<ip>`
2. `grep -E 'sshd.*invalid' /var/log/audit.log` or `grep -E 'sshd.*failed' /var/log/audit.log`