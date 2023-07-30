
# Aurora
- Fully managed relational database compatible with MySQL and Postgres SQL
- Min of 10 GB to a maximum of 64 TB depending on the requirement
- Scales in a few minutes up to a maximum extent of 32 vCPUs, and 244 GiB of RAM
- It supports fifteen replicas for the provision
- For Amazon Aurora, each Read Replica is associated with a priority tier (0-15)
- In the event of a failover, Amazon Aurora will promote the Read Replica that has the highest priority 
  (the lowest numbered tier)
- If two or more Aurora Replicas share the same priority, then Amazon RDS promotes the replica that is largest in size
- If two or more Aurora Replicas share the same priority and size, then Amazon Aurora promotes an arbitrary replica in 
  the same promotion tier