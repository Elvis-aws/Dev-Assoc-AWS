
# Redis vs Memcached
1) latency
- Both Redis and Memcached support sub-millisecond response times. By storing data in-memory they can read data more 
   quickly than disk based databases. Redis is much faster
2) Data partitioning
- Both Redis and Memcached allow you to distribute your data among multiple nodes. This allows you to scale out to 
  better handle more data when demand grows
3) Multithreaded architecture
- Since Memcached is multithreaded, it can make use of multiple processing cores. This means that you can handle more 
  operations by scaling up compute capacity
4) Snapshots
- With Redis you can keep your data on disk with a point in time snapshot which can be used for archiving or recovery
5) Replication
- Redis lets you create multiple replicas of a Redis primary. This allows you to scale database reads and to have highly 
  available clusters
6) Transactions
- Redis supports transactions which let you execute a group of commands as an isolated and atomic operation
7) Pub/Sub
- Redis supports Pub/Sub messaging with pattern matching which you can use for high performance chat rooms, real-time 
  comment streams, social media feeds, and server intercommunication
8) Lua scripting
- Redis allows you to execute transactional Lua scripts. Scripts can help you boost performance and simplify your 
  application
9) Geospatial support
- Redis has purpose-built commands for working with real-time geospatial data at scale. You can perform operations like 
  finding the distance between two elements (for example people or places) and finding all elements within a given 
  distance of a point