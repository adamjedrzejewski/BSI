# Log analysis by a particular service

1. `ssh <user>@<ip>`
2. `grep -i "VSFTPD\|FTP\|XINETD" /var/log/audit.log`