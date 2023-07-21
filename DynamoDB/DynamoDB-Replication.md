
# DynamoDB Replication
- DynamoDB replication is synchronous for multi-az
- Synchronous Replication: When a master node, receives a write transaction, it propagates the changes immediately to 
  its replicas ensuring that the data remains consistent across the main servers and replicas
- DynamoDB replication is asynchronous for global-tables
- Asynchronous Replication: The master node first commits write transactions and then propagates the changes to its 
  replicas