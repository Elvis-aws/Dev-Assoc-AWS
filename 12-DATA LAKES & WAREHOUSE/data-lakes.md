
# AWS Data Lakes - Simplified Big Data Solutions
- Usually big data solutions are complex
# Here are some of the challenges with typical big data solutions:
- How can we make collecting, analyzing (reporting, analytics, machine learning) and visualizing huge data sets easy?
- How to design solutions that scale?
- How to build flexibility while saving cost?
- Data Lakes provides a Single platform with combination of solutions for data storage, data management and data 
  analytics
# AWS Data Lakes - Storage and Ingestion
- AWS Data Lakes makes use of varieties of AWS services for Storage and Ingestion:
# Storage
- Amazon S3 and S3 Glacier provide an ideal storage solution for data lakes
# Data Ingestion
- Streaming data - Amazon Kinesis Firehose
  - Transform and store to Amazon S3
  - Transformation operations - compress, encrypt, concatenate multiple records into one (to reduce S3 transactions cost) 
    and execute lambda functions
- Bulk data from on-premises - AWS Snowball
- Integrate on-premises platforms with Amazon S3 - AWS Storage Gateway
# Amazon S3 Query in Place
- Amazon S3 Query in Place allows you to run your analytics directly from Amazon S3 and S3 Glacier
# Here are some of the important options provided by S3 Select and Glacier Select:
- SQL queries to retrieve subset of data
- Supports CSV, JSON, Apache Parquet formats
- Build serverless apps connecting S3 Select with AWS Lambda
- Integrate into big data workflows
  - Enable Presto, Apache Hive and Apache Spark frameworks to scan and filter data
# Here are some of the important recommendations for S3 Query in Place:
- You want to get quick insights from your cold data stored in S3 Glacier. You want to run queries against archives 
  stored in S3 Glacier without restoring the archives
  - Use S3 Glacier Select to perform filtering and basic querying using SQL queries
  - Stores results in S3 bucket
  - No need to temporarily stage data and then run queries
# Recommendations:
Store data in Amazon S3 in Parquet format
Reduce storage (upto 85%) and improve querying (upto 99%) compared to formats like CSV, JSON, or TXT
Multiple compression standards are supported BUT GZIP is recommended
Supported by Amazon Athena, Amazon EMR and Amazon Redshift
Other options to run Query in Place include: