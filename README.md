# AWS VPC Peering Project

## EWB Cloud Labs - Batch 1

### Project Overview
This project demonstrates secure private communication
between two AWS Virtual Private Clouds (VPCs) using
VPC Peering.

## AWS Services Used
- Amazon VPC
- Amazon EC2
- VPC Peering
- Route Tables
- Security Groups
- Internet Gateway

## Network Architecture

| Resource | CIDR / IP |
|----------|-----------|
| VPC A | 10.10.0.0/16 |
| VPC B | 10.20.0.0/16 |
| Public Subnet A | 10.10.1.0/24 |
| Private Subnet A | 10.10.2.0/24 |
| Private Subnet B | 10.20.1.0/24 |
| App-A | 10.10.2.162 |
| App-B | 10.20.1.247 |

## Project Implementation
1. Created two VPCs with non-overlapping CIDR blocks.
2. Configured public and private subnets.
3. Launched three EC2 instances.
4. Created and accepted a VPC Peering connection.
5. Updated route tables for private communication.
6. Configured security groups.
7. Used SSH ProxyJump for private EC2 access.
8. Tested bidirectional connectivity.
9. Performed failure and recovery testing.
10. Cleaned up AWS resources.

## Connectivity Testing
- Before peering: 100% packet loss.
- After peering: 0% packet loss.
- ICMP blocked: 100% packet loss.
- ICMP restored: 0% packet loss.

## Security
- Application EC2 instances have no public IP.
- SSH access uses a Bastion Host.
- Private SSH keys remain on the local machine.
- Security groups restrict inbound access.

## Project Report
The complete project report is available in this repository.

## Author
Aniket Vivekanand Todkar

EWB Cloud Labs - Batch 1
