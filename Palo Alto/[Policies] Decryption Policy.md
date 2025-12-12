# Decryption Policy Overview

A decryption policy is a set of rules that tells the firewall which encrypted traffic to decrypt and to leave encrypted

<br>

# Decryption Methods

| Decryption Method | Description |
| --- | --- |
| SSL Forward Proxy | Decrypts outbound HTTPS traffic from internal clients to external servers by impersonating the destination site with a trusted enterprise CA certificate |
| SSL Inbound Inspection | Decrypts inbound HTTPS traffic from web servers where the organization owns the TLS certificate and the private key |
| SSH Proxy | The proxy acts as a man-in-the-middle for SSH sessions |