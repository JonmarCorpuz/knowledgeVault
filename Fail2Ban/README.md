# Fail2Ban Overview

Fail2Ban is an open-source IPS that monitors log files for repeated failed login or suspicious activity and then automatically adds firewall rules to block the offending IPs for a period of time

<br>

# Installing Fail2Ban

```Bash
sudo apt -y update && sudo apt install fail2ban -y && sudo systemctl enable --now fail2ban && sudo systemctl start fail2ban
```

