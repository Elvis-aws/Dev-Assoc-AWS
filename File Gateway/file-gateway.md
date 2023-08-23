
# File Gateway
- A file gateway provides a simple solution for presenting one or more Amazon S3 buckets and their objects as a mountable 
  NFS or SMB file share to one or more clients on-premises
- The file gateway is deployed as a virtual machine in VMware ESXi or Microsoft Hyper-V environments on-premises, or in 
  an Amazon Elastic Compute Cloud (Amazon EC2) instance in AWS
- File gateway can also be deployed in data center and remote office locations on a Storage Gateway hardware appliance
- When deployed, file gateway provides a seamless connection between on-premises NFS (v3.0 or v4.1) or SMB (v1 or v2) 
  clients—typically applications—and Amazon S3 buckets hosted in a given AWS Region
- The file gateway employs a local read/write cache to provide low-latency access to data for file share clients in the 
  same local area network (LAN) as the file gateway
- A bucket share consists of a file share hosted from a file gateway across a single Amazon S3 bucket
- The file gateway virtual machine appliance currently supports up to 10 bucket shares