# SSL Forward Proxy Overview

An SSL Forward Proxy decrypts outbound HTTPS traffic from internal clients to external servers by impersonating the destination site with a trusted enterprise CA certificate

* Allows the firewall to inspect and then re-encrypt the traffic before sending it on
* Requires deploying an enterprise CA certificate on the firewall and trusting it on endpoints
* The firewall presents its own certificate to the internal client
* The firewall established a separate TLS session to the external server and sits between the client and the Internet in order to inspect the traffic and enforce security policies