
# Encryption
- You can encrypt your Amazon RDS DB instances and snapshots at rest by enabling the encryption option for your Amazon 
  RDS DB instances
- Data that is encrypted at rest includes the underlying storage for DB instances, its automated backups, read replicas, 
  and snapshots 
- You can only enable encryption for an Amazon RDS DB instance when you create it, not after the DB instance is created
- However, because you can encrypt a copy of an unencrypted DB snapshot, you can effectively add encryption to an 
  unencrypted DB instance
- That is, you can create a snapshot of your DB instance, and then create an encrypted copy of that snapshot