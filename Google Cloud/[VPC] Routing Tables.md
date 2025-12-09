# VPC Routing Table Overview

A VPC routing table is a table that contains the set of all routes that define where packets from that VPC are sent (*Similar to a virtual list of next hop rules*)

* Applied at the VPC level and not per subnet
* Each route contains a destination CIDR and a single next hop
* All ressources within a VPC will consult the routing table of the VPC that it's in for where to send its traffic