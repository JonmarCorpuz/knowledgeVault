# GKE Endpoint Overview

An endpoint in GKE refers to the Kubernetes API server that nodes will use when communicating with the control plane

<br>

# GKE Endpoint Types

## DNS-Based Endpoint

A DNS-based GKE endpoint exposes the control plane via a Google-managed FQDN

* Can be used by clients to connect to the control plane
* The FQDN resolves to Google's infrastructure which can route traffic over secure paths from environments that can reach Google APIs

<br>

## IP-Based Endpoint

An IP-based GKE endpoint exposes the control plane via a public IP, a private IP, or both

* Nodes will always communicate with the public endpoint by default if both private and public endpoints are enabled