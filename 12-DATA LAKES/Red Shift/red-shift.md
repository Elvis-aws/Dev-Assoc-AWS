
# Amazon Redshift
- Redshift is a relational database ( tables and relationships)
# What is the need for another relational database?
- RDS is optimized for online transaction processing
- It is optimized to provide a balance between both reads and write operations
- OLAP workloads have exponentially larger reads on the databases compared to writes
  (Online analytical processing (OLAP) is software technology you can use to analyze business data from different points
  of view. Organizations collect and store data from multiple data sources, such as websites, applications, smart meters, 
  and internal systems)
# The questions are:
- Can we use a different approach to design the database?
- How about creating a cluster and splitting the execution of the same query across several nodes?
- Redshift is a petabyte-scale distributed data ware house based on PostgreSQL
# Three important characteristics of Redshift:
- Massively parallel processing (MPP) - storage and processing can be split across multiple nodes
- Columnar data storage
- High data compression
# Use case
- Run complex queries against data warehouse - housing structured and unstructured data pulled in from a variety of sources

