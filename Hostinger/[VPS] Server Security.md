# VPS Server Security Overview

<br>

# Change the Default SSH Port

```Bash
nano /etc/ssh/sshd_config
```
```Text
Port PORT_NUMBER
#AddressFamily any
#ListenAddress 0.0.0.0
#ListenAddress ::
```
```Bash
sudo systemct restart sshd.service
```

<br>

# Disable Root Login

```Bash
nano /etc/ssh/sshd_config
```
```Text
PermitRootLogin=no
```
```Bash
sudo systemctl restart sshd.service
```

<br>

# Use SSH Keys

```Bash
ssh-keygen -t rsa
```

<br>

# Setup an Internal Firewall 

```Bash
sudo apt-get -y install iptables
```
```Bash
sudo iptables -L -v
```

<br>

# Configure the Uncomplicated Firewall

```Bash
sudo ufw enable
```
```Bash
sudo apt-get -y install ufw
```

<br>

# Set Up Fail2Ban

```Bash
sudo apt-get -y install fail2ban
```
```Bash
sudo systemctl status fail2ban
```

<br>

# Install an Antivirus

<br>

# Use a Malware Scanner