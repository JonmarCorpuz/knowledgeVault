# Private GKE Cluster Overview

A private GKE cluster is where the nodes only use internal IP

* Increases network isolation and security by not having it directly reachable from the public Internet
* Can only be reached through the VPC that it's in (Ex: *via VPN*, *Cloud Interconnect*, *Bastion host*, *etc.*)

<br>

# Internet Connectivity

A private GKE cluster reaches the Internet via NAT (Ex: *Cloud Router*, *etc.*)

* NAT will translate the internal IPs to one or more external IPs on the NAT gateway (*Users can reserve static external IP addresses so that all egress from the private cluster appears from a fixed set of addresses*)