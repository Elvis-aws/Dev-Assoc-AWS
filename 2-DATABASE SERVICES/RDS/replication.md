
# Read Replica
- Amazon RDS Read Replicas provide enhanced performance and durability for RDS database (DB) instances
- They make it easy to elastically scale out beyond the capacity constraints of a single DB instance for read-heavy 
  database workloads
- For the MySQL, MariaDB, PostgreSQL, Oracle, and SQL Server database engines, Amazon RDS creates a second DB instance 
  using a snapshot of the source DB instance
- It then uses the engines' native asynchronous replication to update the read replica whenever there is a change to the 
  source DB instance. Read replicas can be within an Availability Zone, Cross-AZ, or Cross-Region
- On a database instance running with Amazon RDS encryption, data stored at rest in the underlying storage is encrypted, 
  as are its automated backups, read replicas, and snapshots
- If the master database is encrypted, the read replicas are necessarily encrypted
- If the master database is not encrypted, the read replicas cannot be encrypted