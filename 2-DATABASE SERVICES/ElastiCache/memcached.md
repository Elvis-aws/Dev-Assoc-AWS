
# Amazon ElastiCache for Memcached
- Simple caching layer intended for use in speeding up dynamic web applications
  - Pure cache 
  - Non-persistent 
  - Simple key-value storage
- Ideal front-end for data stores like RDS or DynamoDB
- Can be used as a transient session store
- Create upto 20 cache nodes
- Use Auto Discovery to discover cache nodes
# Amazon ElastiCache for Memcached - Limitations
- Backup and restore NOT supported
- Does not support encryption or replication
- Does not support snapshots
- When a node fails, all data in the node is lost
- Reduce impact of failure by using large number of small nodes