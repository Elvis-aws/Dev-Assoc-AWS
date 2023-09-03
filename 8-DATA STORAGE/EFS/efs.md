
# EFS Hybrid Storage
- It is a simple, scalable, fully managed elastic NFS file system for use with AWS Cloud services and on-premises resources
- It is a regional service storing data within and across multiple Availability Zones
- Access
   - EC2 instances can access your file system across AZs, regions, and VPCs using an inter-region VPC peering
   - On-premises servers can access using AWS Direct Connect or AWS VPN
- Storage
   - Amazon EFS Infrequent Access (EFS IA) is a storage class that provides price/performance
- File System Access
  - You control which EC2 instances can access your EFS file system by using VPC security group rules and AWS Identity and 
    Access Management (IAM) policies
  - Use EFS Access Points to manage application access
  - When users attempt to access files and directories, Amazon EFS checks their user IDs and group IDs to verify that each 
    user has permission to access the objects