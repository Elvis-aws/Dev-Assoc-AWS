
# EC2 Placement Groups
- Certain use cases need control over placement of a group of EC2 instances
- Examples are use cases needing:
  - Low latency network communication 
  - High availability
- You can control placement of EC2 instances using EC2 placement groups:
  - Cluster (low network latency )
  - Spread (avoid simultaneous failures)
  - Partition (multiple partitions with low network latency)