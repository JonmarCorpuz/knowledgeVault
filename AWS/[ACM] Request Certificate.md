# Certificate Request Overview

Requesting a certificate in ACM means creating a new SSL/TLS certificate resource for one or more domain names so ACM can issue and manage it for you

* The process includes specifying domain names, choosing a validation method, and then  completing that validation before the certificates moves to the **Issued** state

<br>

# Required Information

| Required Information | Description |
| --- | --- |
| Primary domain name | The FQDN that the clients will connect to, that the certificate will secure and that ACM will validate that you control |
| Validation method | Either DNS validation or Email validation so ACM knows how to verify that the user controls the request domain names |