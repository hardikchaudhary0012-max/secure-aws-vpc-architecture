# secure-aws-vpc-architecture
Secure AWS VPC architecture demonstrating networking and security best practices
# Secure AWS VPC Architecture & Networking

## Project Overview
This is a personal project where I designed a secure AWS Virtual Private Cloud (VPC) to demonstrate cloud networking and security best practices.
Designed a highly available AWS VPC architecture with public and private subnets, ALB, Auto Scaling, NAT Gateways, and secure access to S3 following best practices.

## What I implemented in this architecture

Designed a highly available AWS architecture within a single Region, using two Availability Zones to ensure fault tolerance.

Created a custom VPC with proper network segmentation.

Configured public and private subnets in each Availability Zone.

Deployed an Application Load Balancer (ALB) in the public subnets to distribute incoming traffic across multiple servers.

Launched EC2 instances inside private subnets, ensuring they are not directly exposed to the internet.

Implemented an Auto Scaling Group to automatically scale EC2 instances based on demand.

Set up NAT Gateways in each public subnet to allow private instances to access the internet securely for updates and patches.

Attached an Internet Gateway to the VPC to enable public internet access for the load balancer and NAT gateways.

Configured Security Groups to allow only required inbound and outbound traffic, following the principle of least privilege.

Enabled S3 Gateway Endpoint to allow private resources to securely access S3 without using the public internet.

Designed the architecture to be secure, scalable, and highly available, following AWS best practices.

  <img width="611" height="481" alt="vpc-example-private-subnets" src="https://github.com/user-attachments/assets/eb606df2-dbba-42dd-931e-daf15d333cc0" />


## AWS Services Used
-Amazon VPC
-Availability Zones
-Public Subnets
-Private Subnets
-Internet Gateway
-NAT Gateway
-Application Load Balancer (ALB)
-Amazon EC2
-Auto Scaling Group
-Security Groups
-Amazon S3
-VPC Gateway Endpoint (S3 Endpoint)
