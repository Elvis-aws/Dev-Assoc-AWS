
# What is Data Replication?
- Data replication is the process of creating and maintaining copies of data in multiple locations, systems, or storage 
  environments
# RDS Read Replicas
- DynamoDB replication is synchronous for multi-az
- DynamoDB replication is asynchronous for global-tables
- Read replicas enable increased scalability and database availability in the case of an AZ failure
- Read Replicas allow elastic scaling beyond the capacity constraints of a single DB instance for read-heavy database 
  workloads
- RDS read replicas can be Multi-AZ i.e. set up with their own standby instances in a different AZ
- Load on the source DB instance can be reduced by routing read queries from applications to the Read Replica
- One or more replicas of a given source DB Instance can serve high-volume application read traffic, thereby increasing 
  aggregate read throughput
- Read replicas can also be promoted when needed to become standalone DB instances
- Read replicas are available in RDS for MySQL, MariaDB, PostgreSQL, Oracle, and SQL Server as well as Aurora

# Multi-AZ deployments
- RDS Multi-AZ deployment provides high availability, durability, and failover support
- RDS automatically provisions and manages a synchronous standby instance in a different AZ
- RDS maintains the same endpoint for the DB Instance after a failover, so the application can resume database operation 
  without the need for manual administrative intervention
- Amazon RDS launches a new instance incase no standby instance exist during failover

# DNS Auto Failover
- The dns name remains unchanged
- Standby instance connects to this endpoint
- No manual intervention

# Patching multi-AZ deployments
- To minimize downtime, modify the Amazon RDS DB instance to a Multi-AZ deployment
- For Multi-AZ deployments, OS maintenance is applied to the secondary instance first, then the instance fails over, 
  and then the primary instance is updated
- The downtime is during failover