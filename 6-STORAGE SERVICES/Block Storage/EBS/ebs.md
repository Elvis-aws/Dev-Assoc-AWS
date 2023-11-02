
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
# Solid state drives (SSD): 
- Optimized for transactional workloads involving frequent read/write operations with small I/O size, where the dominant 
  performance attribute is IOPS
  - General Purpose SSD volumes
      - They were designed to be a cost-effective storage option for a wide variety of workloads. Gp2 volumes cover 
        system volumes, dev and test environments, and various low-latency apps. You can combine multiple EBS volume types 
        in a RAID to achieve even higher performance on a single instance. Gp2 volumes are fairly cheap, especially for 
        the balanced performance they provide
  - Provisioned IOPS SSD volumes 
      - They are a special type of volume created to fulfill the needs of very intensive I/O workloads that require very 
        high throughput. They are useful for cases which are latency-sensitive, like large database workloads (e.g., 
        MySQL, Cassandra, MongoDB, and Oracle) and critical business applications that need the kind of sustained 
        performance gp2 volumes can’t achieve. The performance of provisioned IOPS SSD volumes can be set during creation 
        time
# Hard disk drives (HDD):
- They are optimized for large streaming workloads where the dominant performance attribute is throughput. HDD volume 
  types include Throughput Optimized HDD and Cold HDD
  - Throughput Optimized HDD volumes
     - Throughput Optimized HDD (st1) volumes are a type of volume that offers low-cost storage while fulfilling the need 
       for sequential workloads that require more throughput than IOPS. When working with data warehouses, log processing, 
       ETL (extract, transform, load) or AWS EMR, this is a volume type to look into. Keep in mind that this volume type 
       cannot be used as a boot volume. St1, like gp2, relies on burstable performance, and volume size will be the main 
       factor when calculating baseline performance
  - Cold HDD volumes
     - Cold HDD (sc1) volumes, like st1 volumes, provide low-cost storage for workloads that rely on throughput rather 
       than IOPS. Sc1 volumes are primarily used for large amounts of data that is infrequently accessed, or in cases 
       where the cost of storage is the most important factor. Sc1, just like st1, cannot be used as a boot volume and 
       relies on burstable performance