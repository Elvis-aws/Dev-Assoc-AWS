
# EFS
- POSIX compliant file storage system for the EC2 instances (POSIX storage refers to any storage that can be accessed 
  using POSIX filesystem functions)
- Provides a file system interface and concurrent accessible storage for the multiple EC2 instances
- Unlimited system size
- Elastic in nature and can automatically increase or decrease as we add or remove files
- Offers no service level agreement and runs in multiple availability zones
- Encryptes both data at rest by using AWS key management service and in transit by using TLS 1.2
- Stored in multiple availability zones
- Resources that can access the mount point can access the file system
- Offer EFS to EFS replication through AWS DataSync service or any third party tools
- Best for database backups, containers, storage sets, web serving, etc
# Standard storage classes (Recommended)
- EFS Standard and EFS Standard–Infrequent Access, which offer Multi-AZ resilience and the highest levels 
  of durability and availability
- EFS One Zone and EFS One Zone–Infrequent Access, which offer you the choice of additional savings by choosing to save 
  your data in a single Availability Zone
- EFS Standard Storage pricing is $0.30 per GB per month