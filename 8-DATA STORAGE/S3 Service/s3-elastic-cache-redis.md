
# Elastic Cache
- S3 is the persistent store for applications such as data lakes, media catalogs, and website-related content
- These applications often have latency requirements of 10 ms or less
- Many applications, such as media catalog updates require high frequency reads, and consistent throughput
- For such applications, customers often complement S3 with an in-memory cache, such as Amazon ElastiCache for Redis
- This helps to reduce the S3 retrieval cost and to improve performance

# Example
- Consider the real example of an AWS customer who streams media content
- This customer updates their media catalog and channel guides that are consumed by millions of set-top boxes several 
  times a day
- These updates generate over one million read operations per second against 1% of their data stored in S3
- During the updates, they have to sustain latency at < 5 ms. Caching hot objects outside of S3, such as their content 
  catalog, helps this customer meet their transfer performance goals, while also reducing their retrieval and transfer 
  costs