# Module 5 : Storage

Storage types in AWS have been separated into three different categories:

1. Block
2. Object 
3. File

## Block Storage

- In block storage, files are separated into eqal-sized pieces (block) of data.
- Block storage is used for applications that run on Amazon EC2 instances. 

Usages: Operating Systems , 

AMI has the concept of Block Storage enacted

### Amazon EBS Volumnes

Amazon EC2 instances can attach an EBS volume with data.

EBS is one-to-one and cannot be shared with other EC2 or compute instances.
The EBS volume is sitting on the SAN.

Ideal for data that requires retention.

#### EBS Snapshots

- EBS volume (source data) can backup data as a flat file 

#### Instance Store

Allows you to use the physical hardware 
Good for temporary data or caching data that is meant to be temporary. 
Does not support Snapshots and is on the physical server.

## Object Storage

In Object Storage, each object consists of data, metadata and a key.

Object Storage has been around and is really the industry standard for long term memory 


### Amazon Simple Storage Service (S3)

- Storage objects in buckets
- Set permissions to control access to objects
- Choose from a range of storage classes for different use cases

You pick a region and then you can start creating buckets to put files 

#### Storage Classes 

S3 Standard 

- Designed for frequently accessed data
- Stores data in a minimum of three Availability Zones

S3 Standard-IA

- Ideal for infrequently accessed data 
- Similar to S3 standard but has a lower storage price and higher retrieval price

S3 One Zone-IA 

- Storages data in a single Availability Zone
- Has a lower storage price than S3 Standard-IA

S3 Intelligent-Tiering

⚠️ - Not a Storage Class
- Ideal for data with uknown or changing access patterns.
- Requires a small monthly monitoring and automation fee per object

S3 Glacier

- Low-cost storage designed for data archiving
- Able to retrieve objects within a few minutes to hours


## File Storage

In file storage, multiple clients can access data that is stored in shared file folders. 

### Amazon Elastic File System (EFS)

For your Linux Base EC2 instances 

### FSX for Windows File System


## Amazon Relational Database Service

Operate and scale a relational data in the AWS Cloud
Automate time-consuming administrative task
Storage and transmit data securely 

