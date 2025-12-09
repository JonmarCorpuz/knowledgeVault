# Private GKE Endpoint Overview

A private GKE endpoint is the internal IP address of the GKE control plane (Kubernetes API server) that's only reachable from within the VPC that it's in or connected to

* Runs in a dedicated "master" CIDR (**masterIPv4CidrBlock**) and is fronted by an internal passthrough load balancer in the control plane VPC
