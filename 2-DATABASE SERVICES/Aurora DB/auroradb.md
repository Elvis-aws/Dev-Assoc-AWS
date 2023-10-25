
# Aurora
- Fully managed relational database compatible with MySQL and Postgres SQL
- Min of 10 GB to a maximum of 64 TB depending on the requirement
- Scales in a few minutes up to a maximum extent of 32 vCPUs, and 244 GiB of RAM
- It supports fifteen replicas for the provision
- Each Read Replica is associated with a priority tier (0-15)
- In the event of a fail-over, Amazon Aurora will promote the Read Replica that has the highest priority
- If two or more Replicas share the same priority, then Amazon RDS promotes the replica that is largest
- If two or more Replicas share the same priority and size, then Aurora promotes an arbitrary replica
# Amazon Aurora Serverless
- Aurora Serverless is an on-demand, auto-scaling configuration for Amazon Aurora, where the database will 
  automatically start up, shut down, and scale capacity up or down based on your application's needs
- You pay on a per-second basis for the database capacity you use when the database is active and migrate between standard 
  and serverless configurations with a few clicks in the Amazon RDS Management Console
# Amazon Aurora
- Aurora is a relational database built for the cloud, that combines the performance and availability of traditional 
  enterprise databases with the simplicity and cost-effectiveness of open source databases
- Aurora is up to five times faster than standard MySQL databases and three times faster than standard PostgresSQL
- It's not a complete auto-scaling solution and neither is it fully managed like Aurora serverless
- You cannot promote an Aurora Read Replica to a standalone DB instance