# SSL Inbound Inspection Overview

An SSL Inbound Inspection is a decryption method that applies for inbound HTTPS traffic from web servers where the organization owns the TLS certificate and the private key

* The firewall will terminate and re-encrypt the incoming HTTPS traffic for inspection

<br>

# SSL Inbound Inspection Workflow

1. Client initiates an HTTPS connection to a web server on the Internet

For example
```Text
https://www.victim.com
```

2. The firewall will match a decryption policy by evaluating the source zone, destination zone, destination address, service, and decryption rule

3. The firewall will then respond to the client by presenting the real server certificate that's signed by a trusted CA
* The client will believe it's talking to the real server 

4. The firewall proves private key ownership
* The client will send an encrypted session key and the firewall will decrypt it using the private key
* The TLS handshake should complete successfully