
# AWS storage services
- There are three main cloud storage types: object storage, file storage, and block storage
# Amazon Simple Storage Service (S3)
- Object storage with industry-leading scalability, availability, and security for you to store and retrieve any amount 
  of data from anywhere
# Amazon Elastic File System (EFS)
- A simple, serverless, elastic, set-and-forget file system for you to share file data without managing storage
# Amazon FSx
- Fully managed, cost-effective file storage offering the capabilities and performance of popular commercial and 
  open-source file systems
# Amazon Elastic Block Store (EBS)
- Easy to use, high-performance block storage service for both throughput and transaction-intensive workloads at any 
  scale
# Amazon File Cache
- High-speed cache for datasets stored anywhere, accelerate cloud bursting workloads

# Why use EFS instead of EBS?
- Like EBS, EFS also offers high durability. However, the main difference lies in scalability. EFS volumes can scale up 
  quickly and automatically to meet abrupt spikes in workload demand and scale down with a decreased load. This makes 
  EFS more flexible and better at handling dynamic workloads than EBS
# When should I choose EFS over S3?
- The choice between AWS S3 and EFS depends on the project's requirements. Use AWS S3 for scalable, cost-effective object 
  storage, ideal for static assets and backups. EFS is suitable for dynamic, shared file storage, ensuring file consistency 
  and supporting databases and content management systems
# What is the difference between EFS and FSx?
- EFS is better for applications designed for heterogeneous environments and those that run on Linux systems. It uses NFS, 
  one of the first network file sharing protocols native to Unix and Linux. Windows has long provided an NFS client and 
  server. Some Windows applications might not work on EFS or be feature-complete without access to a native Windows SMB 
  file share
- As a Windows-based service, FSx runs the integrated SMB server built into the OS with storage built on NTFS and supports 
  AD users, access control lists, groups and security policies. These features enable FSx to support multi-AZ deployments 
  using Microsoft's DFS, along with the ability to synchronize file shares in different AZs and configure automatic 
  failovers. FSx supports other Windows security features, such as data encryption at rest and in transit, along with 
  Amazon security services