
# Cluster
- Instances in EC2 Cluster Placement Group are optimized for low latency network communication between EC2 instances
- EC2 instances are placed near to each other in single AZ
- This provides High Network Throughput: EC2 instances can use 10 Gbps or 25Gbps network
- Use Case Example: 
  - Big Data or High Performance Computing needing extreme low latency
- However, the disadvantage is Low Availability (Rack crashes => All EC2 instances fail)