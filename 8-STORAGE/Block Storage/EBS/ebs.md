
# EBS
- Persistent block-level storage for the EC2 instances
- For workloads that require the lowest latency data access
- Can manually increase or decrease the memory size
- Has an availability of 99.99%
- Encryptes both data at rest and in transit through the EBS encryption that uses AWS Key management service
- Stored in a single availability zone
- IAM roles, policies, or Security groups
- Offers durable snapshot capabilities
- Suitable for boot volumes, transaction and NoSQL databases, data warehousing, and ETL operations
# EBS volumes are AZ locked
- When you create an EBS volume, it is automatically replicated within its Availability Zone to prevent data loss due to 
  the failure of any single hardware component
# EBS Volume Types
- Solid state drives (SSD): Suited for applications requiring high IOPS (Input output per second) with heavy transactional 
  work load 
  - General Purpose SSD volumes 
  - Provisioned IOPS SSD volumes 
  - Hard disk drives (HDD):
- Throughput Optimized HDD volumes: Throughput optimization maximizes the rate of materials progressing through the 
  production process by making the best use of available resources
  - Cold HDD volumes
  - Optimized HDD