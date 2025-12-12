# SSH Proxy Overview

An SSH Proxy is a decryption method for depcrypting SSH traffic so that the firewall can inspect interactive sessions while also controlling tunneling and port-forwarding

* The firewall acts as a man-in-the-middle SSH server to the client and as a client to the SSH server
* The firewall can enforce policies while sitting between the SSH server and client (*Which users can connect*, *Which commands are allowed*, *Whether tunneling and port forwarding is permitted*, *etc.*)
* The firewall inspects and controls SSH usage to ensure that users can't create arbitrary tunnels, bypass firewalls, or run risky commands unnoticed