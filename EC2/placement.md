
# EC2 Placement
- EC2 Placement groups determine how the instances are placed on the underlying hardware
- Types of placement groups
# Cluster:
- Cluster – packs instances close together inside an Availability Zone
- This strategy enables workloads to achieve the low-latency network performance necessary for tightly-coupled node-to-node 
  communication that is typical of HPC applications
- This is not suited for distributed and replicated workloads such as Hadoop
# Partition: 
- Spreads instances across logical partitions, ensuring that instances in one partition do not share underlying hardware 
  with instances in other partitions
- This strategy is typically used by large distributed and replicated workloads, such as Hadoop, Cassandra, and Kafka
# Spread: 
- Strictly places a small group of instances across distinct underlying hardware to reduce correlated failures
- Can span multiple Availability Zones in the same region
- Spread level placement groups provide access to distinct hardware
- Spread placement groups are recommended for applications that have a small number of critical instances that should 
  be kept separate from each other