
# EBS
- Amazon Elastic Block Store (Amazon EBS) provides block level storage volumes for use with EC2 instances
- EBS volumes behave like raw, unformatted block devices
- You can mount these volumes as devices on your instances
- They persist independently of the life of the instance
- You can create a file system on top of these volumes
- You can dynamically change the configuration of a volume attached to an instance
- They are particularly well-suited for use as the primary storage for file systems, databases
- They are well suited to both database-style applications that rely on random reads and writes, and to 
  throughput-intensive applications that perform long, continuous reads and writes
- Volume storage for all EBS volume types is charged by the amount of GB you provision per month
- Costs increase for EBS volumes that support additional input/output operations per second (IOPS) and throughput
- For EBS General Purpose SSD (gp2) volumes, the charges are $0.10 per GB-month of provisioned storage