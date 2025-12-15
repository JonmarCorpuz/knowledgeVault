# EC2 Instance Connect Endpoint Overview

An EC2 Instance Connect Endpoint is a managed entry point in a VPC that lets users connect to EC2 instances over SSH or RDP without giving their instances within that subnet a public IP address or running a bastion host

* Acts as a TCP proxy that will forward the authenticated user's traffic privately to their instance
* The user can reach using their IAM-authenticated AWS CLI or console session