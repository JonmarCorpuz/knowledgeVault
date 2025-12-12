# Passthrough Network Load Balancer Overview

A Passthrough Network Load Balancer distributes traffic among backends in the same region as the load balancer

* Operates on Layer 4 of the OSI model
* Forwards packets directly to the destined backend server without acting as a full proxy (Not considered as a proxy)
* Load balancer connections are terminated at the backends and the responses go directly to the clients rather than passing back through the load balancer

