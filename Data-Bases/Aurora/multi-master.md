
# multi-master DB cluster
- In a multi-master cluster, all DB instances can perform write operations
- There isn't any failover when a writer DB instance becomes unavailable, because another writer DB instance is immediately
  available to take over the work of the failed instance
- AWS refers to this type of availability as continuous availability, to distinguish it from the high availability 
  (with brief downtime during failover) offered by a single-master cluster
- For applications where you can't afford even brief downtime for database write operations, a multi-master cluster can 
  help to avoid an outage when a writer instance becomes unavailable
- The multi-master cluster doesn't use the failover mechanism, because it doesn't need to promote another DB instance to
  have read/write capability