
# Amazon Redshift
- Redshift is a relational database ( tables and relationships)
# What is the need for another relational database?
- RDS is optimized for online transaction processing
- It is optimized to provide a balance between both reads and write operations
- OLAP workloads have exponentially larger reads on the databases compared to write
  (Online analytical processing (OLAP) is software technology you can use to analyze business data from different points
  of view. Organizations collect and store data from multiple data sources, such as websites, applications, smart meters, 
  and internal systems)
# The questions are:
- Can we use a different approach to design the database?
- How about creating a cluster and splitting the execution of the same query across several nodes?
- Redshift is a petabyte-scale distributed data warehouse based on PostgresSQL
# Three important characteristics of Redshift:
- Massively parallel processing (MPP) - storage and processing can be split across multiple nodes
- Columnar data storage
- High data compression
# Use case
- Run complex queries against data warehouse - housing structured and unstructured data pulled in from a variety of 
  sources
# Amazon Redshift AQUA 
- It is a new distributed and hardware-accelerated cache that enables Amazon Redshift to run up to 10x faster than other 
  enterprise cloud data warehouses by automatically boosting certain types of queries
- It is available with the RA3.16xlarge, RA3.4xlarge, or RA3.xlplus nodes at no additional charge and with no code changes
# Cross account data share
- Cross-account data sharing is a two-step process
  - First, create a datashare and adds objects, and gives access to the consumer account
  - Second, authorize sharing data for the specified consumer
- You can do this from the Amazon Redshift console
# Video
- https://www.youtube.com/watch?v=IAagaCN4CIk
- https://www.youtube.com/watch?v=CPJgliVQZu4