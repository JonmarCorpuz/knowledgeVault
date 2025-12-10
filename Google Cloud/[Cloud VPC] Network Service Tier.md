# VPC Network Service Tier Overview

A network service tier is a setting that controls what kind of underlying network Google will use to carry the traffic between resoources and the Internet

<br>

# Service Tiers

## Premium

* User traffic enters Google's network at the closest point of presence and then stays on Google's private global backbone as far as possible before reaching your VPC (Vice versa for egress traffic)
* Provides lower latency and higher throughput by reducing the number of hops and congestion

<br>

## Standard

* User traffic will use transit ISP/public internet paths for a larger portion of the journey
* Google will typically only carry user traffic within the same region that the user's resource is in before handing it off
* Suitable for cost-sensitive and regional workloads by providing the same performance similar to otypical public-cloud/ISP routing but at a lower egress price compared to the Premium tier