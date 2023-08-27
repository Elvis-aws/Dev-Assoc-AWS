
# Multi-AZ
- When you provision an RDS Multi-AZ DB Instance, Amazon RDS automatically creates a primary DB Instance and synchronously 
  replicates the data to a standby instance in a different Availability Zone (AZ)
- Each AZ runs on its own physically distinct, independent infrastructure, and is engineered to be highly reliable
- Running a DB instance with high availability can enhance availability during planned system maintenance, and help protect 
  your databases against DB instance failure and Availability Zone disruption
- In the event of a planned or unplanned outage of your DB instance, Amazon RDS automatically switches to a standby replica 
  in another Availability Zone if you have enabled Multi-AZ
- The time it takes for the failover to complete depends on the database activity and other conditions at the time the 
  primary DB instance became unavailable
- Failover times are typically 60–120 seconds

# Read Replica
- Amazon RDS Read Replicas provide enhanced performance and durability for Amazon RDS database (DB) instances
- They make it easy to elastically scale out beyond the capacity constraints of a single DB instance for read-heavy 
  database workloads
- You can create one or more replicas of a given source DB Instance and serve high-volume application read traffic from 
  multiple copies of your data, thereby increasing aggregate read throughput
- Read replicas can also be promoted when needed to become standalone DB instances
- Read replicas are available in Amazon RDS for MySQL, MariaDB, PostgreSQL, Oracle, and SQL Server as well as Amazon Aurora 
- Amazon RDS creates a second DB instance using a snapshot of the source DB instance
- It then uses the engines' native asynchronous replication to update the read replica whenever there is a change to the 
  source DB instance
- The read replica operates as a DB instance that allows only read-only connections; applications can connect to a read 
  replica just as they would to any DB instance. Amazon RDS replicates all databases in the source DB instance