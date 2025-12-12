# Backend Overview

A backend in a Cloud Load Balancer is the actual set of endpoints that'll receive traffic from the load balancer

* Defines how traffic is distributed
* Specifies which health check to use
* Indicates if session affinity is used
* Mentions which other services are used (*Cloud CDN*, *IAP*, *etc.*)

<br>

# Backend Services

## Instance Groups

## Network Endpoint Groups

A NEG is a logical group of individual network endpoints that a load balancer can send traffic to

* A configuration object that specifies a group of backend endpoints or services (Commonly used for deploying services in GKE)

| NEG Types | Description |
| --- | --- |
| Zonal | |
| Internet | |
| Serverless | |
| Private Service Connect | |
| Hybrid Connectivity | |

<br>

## Backend Cloud Storage Bucket