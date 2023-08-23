
# Data Sync (Migration)
- AWS DataSync is a cloud-based service that streamlines the process of transferring data to and from AWS
- It also facilitates the movement of data between on-premises storage, edge locations, and other cloud platforms
- It supports VPC endpoints for moving files securely into your Amazon VPC
- Can be used to copy files into EFS
- It allows you to store data instantly in any S3 storage class
- You don’t need to apply lifecycle policies or transfer data manually to S3

# AWS DataSync can copy data from:
- Network File System (NFS) file servers
- Server Message Block (SMB) file servers
- Hadoop Distributed File System (HDFS)
- Object storage systems
- Amazon Simple Storage Service (Amazon S3) buckets
- Amazon EFS file systems
- Amazon FSx
- AWS Snowcone devices
- Google Cloud Storage buckets
- Azure Files
# Attributes
- DataSync fully automates the data transfer
- It comes with retry and network resiliency mechanisms, network optimizations, built-in task scheduling, monitoring via 
  the DataSync API and Console, and CloudWatch metrics, events, and logs that provide granular visibility into the transfer 
  process
- DataSync performs data integrity verification both during the transfer and at the end of the transfer