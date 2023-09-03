
# EBS
- Persistent block-level storage for the EC2 instances
- Best for workloads that require the lowest latency data access from the single EC2 instance
- 16 TiB for single volumne
- Can manually increase or decrease the memory size. We can attach and detach additional volumes to and from EC2 
  instances to offer scalability
- Has an availability of 99.99%
- Encryptes both data at rest and in transit through the EBS encryption that uses AWS Key management service - Client 
  management keys
- Stored in a single availability zone
- IAM roles, policies, or Security groups
- Offers durable snapshot capabilities
- Suitable for boot volumes, transaction and NoSQL databases, data warehousing, and ETL operations
# EBS volumes are AZ locked
- When you create an EBS volume, it is automatically replicated within its Availability Zone to prevent data loss due to 
  the failure of any single hardware component