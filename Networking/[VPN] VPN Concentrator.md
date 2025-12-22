# VPN Concentrator Overview

A VPN concentrator is a dedicated network device or service that terminates and manages a large number of VPN tunnels

* Essentially a high-capacity VPN gateway designed for scalability, central management, and strong authentication
* Provides secure remote access for users over the internet into an internal network
* Builds and maintains individual encrypted tunnels for each connection
* Centrally handles key exchange, encryption, decryption, and user authentication
* Often integrated with identity stores so that only authenticated and authorized users can bring up tunnels and reach specific subnets

<br>

# How it Works

* Sits at or near the edge of a network (*Usually next to or integrated with the firewall*)
* Acts as the VPN server endpoint that the remote clients will establish a tunnel to
* Once a tunnel is established, the VPN connector will route traffic into the internal network according to policy
