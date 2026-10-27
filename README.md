AWS Transit Gateway – Cross-Region Connectivity

Project Overview

Implemented cross-Region connectivity between three Amazon VPCs across Mumbai and Singapore using AWS Transit Gateway and inter-Region peering.

Architecture

- Mumbai Region ("ap-south-1")
  - A-VPC: "10.10.0.0/16"
  - B-VPC: "10.20.0.0/16"
- Singapore Region ("ap-southeast-1")
  - C-VPC: "10.30.0.0/16"

Each VPC contains an EC2 instance launched in a private subnet.

AWS Services Used

- Amazon VPC
- AWS Transit Gateway
- Transit Gateway Peering
- Amazon EC2
- VPC Route Tables
- Security Groups

Implementation

1. Created three VPCs across two AWS Regions.
2. Launched EC2 instances in private subnets.
3. Attached the VPCs to their respective Transit Gateways.
4. Established cross-Region Transit Gateway peering.
5. Configured static routes and VPC route tables.
6. Verified connectivity using private IP addresses.

Outcome

Successfully tested private IP connectivity between EC2 instances in Mumbai and Singapore.

Key Learnings

- Cross-Region Transit Gateway peering.
- Transit Gateway routing and VPC route tables.
- Private network connectivity and ICMP troubleshooting.
