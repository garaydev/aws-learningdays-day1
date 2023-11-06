## Module 3 - Compute

Amazon Elastic Compute Cloud (Amazon EC2)

EC2 is basically a virtual machine in the cloud

🧪- Amazon Machine Image (AMI) are responsible for housing the following sections:

Operating System
Storage mappings
Permissions

Block Device Mapping is where the Operating System goes under the AMI

EC2 Instances than have a Root volumme 

4 ways to get AMI

- Quick Start
- Marketplace
- Community

Hardware is the Instance Types. Instance Types include:

General Purpose (M types)
Compute Optimized (C Types)
Memory Optimized (R Types (RAM))
Accelerated computing (P types, G types, F types)
Storage Optimized (D types)

There are sizes to each of these Instance Types as well 

EC2 Pricing 

On-Demand

- No upfront costs or minimum contracts
- Ideal for short-term, irregular workloads

Spot 

- Ideal for workloads with flexible start and end times
- Great for batch processing

Reserved 

- Provides a biling discount over On-Demand pricing

Compute Savings Plans 

- Offers better pricing and it's newer  
🧪 - One or Three Years term commient for Reserved and Compute Savings Plans 

Dedicated Instance 

- An EC2 Instance that runs in a VPC on hardware for single customer
- Higher cost compared to Standard Amazon EC2 instances
- You DO NOT have an understand of where the EC2 instances are installed

Dedicated Host 

- A physical server with EC2 instance capacity for a single customer 
- Most expensive Amazon EC2 service
- Can determine the underlying components and hardware (the OS and the space on the rack)

## Auto Scaling

- Manual Scaling vs. Auto Scaling

## Elastic Load Balancers (ELBs)

- Provide a single point of contract for your Auto Scaling group

There are several types of load balancing

- Classic
- Network Load Balancer
- Application Load Balancer

You can combine Load Balancers to Auto Scaling Groups and setup triggers to react to the usage of your applications.

# Amazon Simple Notification Service (SNS)

Messages are published to a queue. 

Publish updates from multiple topics

A one to many relationship

## Amazon Simple Queue Service (SQS)

Send, storge, and receive messages between software components

This follows the subscriber model that requires a pull of the data. 

## Serverless Computing 

Computing with vritual servers vs. Serverless computing 

### AWS Lambda

Run code without provisioning or managing servers
Pay only for compute time while code is running

### AWS Containers 

One host with multiple containers

We are virtualaizing the Operating System to get away from the OS dependency. 

### Amazon Elastic Container Service (amazon ECS)

ECS stands for Elastic Container Service and Amazon sets up all of the container management

### Amazon Elastic Kubernetes Service (Amazon EKS)

### AWS Fargate 

- Run serverless containers with amazon ECS or Amazon EKS
- Pay only for the resources you use

