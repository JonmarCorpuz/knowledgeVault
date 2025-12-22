# Certificate Authority Overview

CAs are trusted entities that are responsible for issuing, signing, and managing digital certificates that bind public keys to verified entities

* Verifies the identity of certificate applicants and then issues X.509 certificates signed with the CA's private key
* Acts as the root of trust meaning that the clients will trust the CA's root certificate so certificates chained to it are trusted transitively
* Maintains CRLs or OCSP responders to notify clients of revoked certificates

<br>

# Certificate Authority Hierarchy

## Root Certificate Authority

<br>

## Intermediate/Subordinate Certificate Authority