# Free Range Routing Overview

FRRouting is an open-source routing software suite that turns a Linux or Unix system into a full-feature IP router

* Provides a modular routing stack that runs in user space on Unix-like OSes
* Can be used in dual-stack environments (IPv4 and IPv6)
* Implements common routing protocols (*BGP*, *OSPF*, *RIP*, *IS-IS*, *PIM*, *LDP*, *VRRP*, *etc.*)

<br>

# Install FRRouting

## Ubuntu Server

Install FRRouting
```Bash
sudo apt -y update
curl -s https://deb.frrouting.org/frr/keys.asc | sudo gpg --dearmor -o /usr/share/keyrings/frr.gpg
echo "deb [signed-by=/usr/share/keyrings/frr.gpg] https://deb.frrouting.org/frr noble frr-stable" | sudo tee /etc/apt/sources.list.d/frr.list
sudo apt -y update
sudo apt -y install frr frr-pythontools
```

Launch FRRouting
```Bash
sudo vtysh
```