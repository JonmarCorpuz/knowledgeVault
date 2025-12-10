# Application Load Balancer Overview

An Application Load Balancer is a proxy-based L7 load balancer that allows users to run and scale their application services 

* Distributes HTTP and HTTPS traffic to backends hosted on GCP (*GCE*, *GKE*, *etc.*)

<br>

# External Application Load Balancer

| Deployment Mode | Network Service Tier | Load Balancing Scheme |
| --- | --- | --- |
| Global External | Premium | EXTERNAL_MANAGED |
| Regional External | Premium or Standard | EXTERNAL_MANAGED |
| Classic | Global in Premium Tier or Regional in Standard Tier | EXTERNAL* |

<br>

# Internal Application Load Balancer

| Deployment Mode | Network Service Tier | Load Balancing Scheme |
| --- | --- | --- |
| Regional internal | Premium | INTERNAL_MANAGED |
| Cross-regiona internal* | Premium | INTERNAL_MANAGED |