
# EC2 Placement
- EC2 Placement groups determine how the instances are placed on the underlying hardware
# Types of placement groups
- Cluster: Clusters instances into a low-latency group in a single AZ
- Partition: Spreads instances across logical partitions, ensuring that instances in one partition do not share 
  underlying hardware with instances in other partitions
- Spread: Strictly places a small group of instances across distinct underlying hardware to reduce correlated failures
  Can span multiple Availability Zones in the same region