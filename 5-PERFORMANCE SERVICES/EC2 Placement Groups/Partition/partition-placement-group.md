
# Partition
- In large distributed and replicated workloads (HDFS, HBase, and Cassandra), EC2 instances need to be divided into 
  multiple groups with:
- Low latency communication between instances in a group
- Each group is placed on a different rack
- A partition is a group of EC2 instances. In a EC2 Partition Placement Group, each partition will be placed on a 
  different rack
# Features:
- You can choose the partition where EC2 instance is launched into
- Can be spread across different AZs in same region
- Maximum of seven partitions per Availability Zone per group
# EC2 Placement Groups - Certification Tips
- Insufficient capacity error can happen when:
  - New instances are added in (OR)
  - More than one instance type is used (OR)
  - An instance in placement group is stopped and started
- If you receive a capacity error:
  - Stop and start all instances in the placement group (OR)
  - Try to launch the placement group again 
  - Result: Instances may be migrated to a rack that has capacity for all the requested instances
# Recommendation:
- Have only one instance type in a launch request AND
- Launch all instances in a single launch request together