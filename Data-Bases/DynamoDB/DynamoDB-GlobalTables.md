
# DynamoDB Global Tables
- For disaster recovery global tables are important
- Geographical distribution of customer base to reduce latency
- DynamoDB streams must be enabled 
- Changes made to the main table will be copied to the stream
- There is usually latency with replication as tables are further from each other
- Decoupled and asynchronous replication ensure replicas operate without any cross-region dependency
- Last writer wins mechanism due to latest write time stamp