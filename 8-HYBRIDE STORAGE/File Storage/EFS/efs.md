
# EFS Storage
- Automatic scaling
- Encryptes both data at rest by using AWS key management service and in transit by using TLS 1.2
- POSIX compliant (POSIX storage refers to any storage that can be accessed using POSIX filesystem functions)
- Supports NFS version 4.1
- Use with AWS Cloud services and on-premises resources
- Offer EFS to EFS replication through AWS DataSync service or any third party tools
- Best for database backups, containers, storage sets, web serving, etc
- Regional service storing data within and across multiple Availability Zones
- Access
   - EC2 instances can access your file system across AZs, regions, and VPCs
   - On-premises servers can access using AWS Direct Connect or AWS VPN
- Storage
   - Amazon EFS Infrequent Access (EFS IA) is a storage class that provides price/performance
- File System Access
  - Use VPC security group rules and IAM policies
  - Use EFS Access Points to manage application access
  - Amazon EFS checks user IDs and group IDs to verify that each user has permission to access the objects

# Standard storage classes (Recommended)
- EFS Standard and EFS Standard–Infrequent Access, which offer Multi-AZ resilience and the highest levels 
  of durability and availability
- EFS One Zone and EFS One Zone–Infrequent Access, which offer you the choice of additional savings by choosing to save 
  your data in a single Availability Zone
- EFS Standard Storage pricing is $0.30 per GB per month
- EFS Lifecycle
  - Automatic object transitioning