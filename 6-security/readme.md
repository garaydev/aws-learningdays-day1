# Module 6: Security 

## AWS Shared Responsibility

Tiers going down:

AWS responsibilities

1. Software
2. Compute - Storage - Database - Networking
3. Hardware/AWS Global Infrastructure
4. Regions - Availability Zones - Edge Locations

You are responsible for security IN the cloud, AWS is responsible for security OF the cloud. 

Customers

Customer Data (At-Rest and In-Transit)
Platform, Applications, Identity and Access Management
Operation Systems, Network and Firewall Configuration
Client-side Data Encryption, Server-side Encryption, Networking Traffic Protection 

## AWS Security

### Identity and Access Management

AWS IAM allows you to manage access to AWS services and resources.

IAM Policy
IAM group
IAM role
MFA

A group is no more than a way to manage a category of users.

AWS follows a implied deny 

A Role is an assumed rule and these are really temporary 

A project?

#### IAM Policy

This sample IAM policy allows permission to view a list of objects in the Amazon S3 bucket with ID 'awsdoc-example-bucket' and also access them. 

JSON is a good example

Expolit deny means you really cannot 

### IAM Groups 

An IAM group is a collection of IAM users. 

Best Practicve: attach IAM policies to IAM groups, rather than to individual IAM users.

### IAM Roles 

A IAM Role is an identity that you can assume to gain temporary access to permissions.

### AWS Organizations

- AWS Organizations helps customers consolidate and manage multiple AWS accounts in a central location.
- Use service control policies (SCPs) to centrally control permissions for accounts in your organization.
  
Organization Units are the folders that contain different accounts. Service Control Policies just restrict. They say what you cannot do.


## AWS Artifacts

This allows you to sign online agreements. You can download the 

### Customer Compliance Center 

Allows you to see how 


## AWS Web Application Firewall

Allows you to put rules in front of your application under EC2. 

You can do rate limiting , Block IP addresses from certain countries,

## AWS Shield 

Infrastructure layer security to prevent DDoS attacks. AWS Shield provide protection against distributed denial of service (DDoS) attacks.

Shield Standard is free while Shield  Advance is not. 

There is Cloud integration to CloudFront 

## Amazon Inspector 

Amazon Inspector allows you to perform automated security assements on your applications. 

## AWS Key Management Services 

Helps customers perform encryption oerations through the use of cryptographic keys. 
You can choose the specific levels of access

## AWS GuardDuty 

Provides intelligent threat detection for AWS products and services.