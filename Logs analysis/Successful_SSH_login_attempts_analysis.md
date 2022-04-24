# Successful SSH login attempts analysis

1. `ssh <user>@<ip>`
2. `grep -i opened /var/log/audit.log | grep -i ssh | grep CS`