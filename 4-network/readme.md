# Module 4: Network 

## Amazon Virtual Private Cloud (Amazon VPC)

- Enables you to launch resources in a virtual network that you can define.
- VPCs are bound by the region but span all of the Availability Zone within that one Region.

- You define the IP Range, the CIDRs, the Subnets, 

### Types of Subnets

Public and Private subnets are the only types that exist in AWS

- A public is defined as a subnet that allows the resources inside of it to the Internet and those 

- A private subnet is not allowed to access the internet directly or indirectly. A good example of a private subnet is your database.

### Gateways

Internet Gateways are components that you provision and attach to the VPC to allow traffic to the Internet. 

0.0.0.0/24 goes to the your Internet Gateway

You need a VPG in your VPC to create a VPN. Wow.

The name of the service for VPNs is called Site-To-Site VPNs. 
- VPG , Virtual Private Gateway 
- VPC, Virtual Private Cloud

## AWS Direct Connect

This takes time and cost the most but functions as a direct , fiber connection to the AWS backbone and infrastructure.

## Network Access Control List (ACL)

- These are virtual firewalls for a subnet that allows you to control the network traffic coming in.

Custom network ACLS deny all inbound and outbound traffic. 

If you let it in, you better let it out. A good example is checking your passport.

ACLs read in order and therefore 

## Security Groups

- A security group is required for EC2 instances. A security group is stateful. By default a SG denies all inbound traffic and allows all outbound traffic.. 

Network ACLs and Security groups play a big in how EC2 communication is allowed across the Internet. 

## Amazon Route 53 

DNS or Domain Name System are controlled by 

You can connect Route 53 to your VPC or Virtual Private Cloud

Global Routing Policies allows 