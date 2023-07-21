
# Instant Store
- An instance store provides temporary block-level storage for your instance
- This storage is located on disks that are physically attached to the host computer
- Ideal for temporary storage such as buffers, caches, scratch data, and other temporary content 
- The virtual devices for instance store volumes are ephemeral[0-23]
- Instance store volumes are included as part of the instance's usage cost
- A common strategy with instance store volumes is to persist necessary data to Amazon S3 regularly as needed
- For persistence, create an EBS volume, attach it to your instance, and copy the data from the instance store volume 
  to the EBS volume on a periodic basis


# EC2 EBS Volumes
- Amazon Elastic Block Store (EBS) is a high-performance block storage solution designed to be used with EC2 instances
- It works by giving the user access to a multitude of small network-attached blocks, each of which is presented as a 
  simple volume
- You can create an EBS snapshot, effectively making a backup of your entire volume
# AWS EBS Volume Types
- Solid state drive (SSD) volumes
    - Optimized for transactional workloads involving frequent read/write operations
    - They include 
        - General Purpose SSD (gp2, gp3)
            - Recommended for most workload
            - System boot volumes
            - low latency
            - 1GB to 16TB
            - Cheap
        - Provisioned IOPS SSD (io1, io2)
            - Critical business application that requires sustained performance
            - Large database workloads such as MongoDB, PostgresSQL, Oracle
            - 4GB to 16TB
            - Expensive
- Hard disk drive (HDD) volumes
    - Optimized for large streaming workloads where the dominant performance attribute is throughput
    - HDD volume types include 
        - Throughput Optimized HDD (st1) 
            - Big Data
            - Data lake
            - Data Warehouse
            - Log processing
            - Cant be used as boot volume
        - Cold HDD (sc1)
            - Lowest storage cost
            - Not a boot volume
            - Large infrequently accessed data
- Previous generation volumes
    - Suited for workloads with small datasets where data is accessed infrequently