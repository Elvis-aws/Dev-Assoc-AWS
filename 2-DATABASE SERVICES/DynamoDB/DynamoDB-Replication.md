
# DynamoDB Replication
- DynamoDB replication is synchronous for multi-az
- DynamoDB replication is asynchronous for global-tables
- When a master node, receives a write transaction, it propagates the changes immediately to 
  its replicas ensuring that the data remains consistent across the main servers and replicas