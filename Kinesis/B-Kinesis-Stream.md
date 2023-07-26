
# Kinesis
- There are several services that make up the kinesis family
  - Kinesis data stream
  - Kinesis Data Firehose
  - Kinesis Video Streams
  - Kinesis Data Analytics

# Kinesis data stream
- This service allows you to capture and store data streams in real-time
- Data Collection: Kinesis Data Streams enables you to ingest large volumes of streaming data from producers
- Shards: Data streams are divided into shards, which are the basic units of data storage and throughput capacity
  Each shard represents a sequence of data records in a stream and can handle a specific amount of data throughput
- Real-time Data Processing: After data is ingested into a Kinesis Data Stream, you can process it in real-time using 
  consumer applications. These applications can be implemented using AWS Lambda, the Amazon Kinesis Client Library (KCL), 
  or other compatible tools and frameworks
- Data Retention: Kinesis Data Streams allows you to control the retention period for data in the stream. This means 
  you can specify how long data should be stored in the stream before it expires. By default, the data is stored in shards 
  for 24 hours. You can increase the time to 7 days of retention
- Data Analytics: Kinesis Data Streams integrates with other AWS services like Amazon Kinesis Data Analytics, Amazon 
  Elasticsearch, and Amazon SageMaker, enabling you to perform real-time data analytics, derive insights, and build 
  machine learning models on streaming data
- Data Replication and Durability: The service replicates data across multiple Availability Zones within an AWS region 
  to ensure high availability and durability of your data
- Scalability: Kinesis Data Streams can scale automatically to handle varying data ingestion rates, making it suitable 
  for applications with fluctuating workloads
- Pay only for what you use with Kinesis Data Streams, starting as low as $0.015 per hour. With the on-demand mode, 
  you don't need to worry about over-provisioning
- Data ordering: Ordering of records at the shard level, as well as the ability to read and/or replay records in the 
  same order to multiple Amazon Kinesis Applications

# Kinesis Data Firehose
- This service is designed for real-time data ingestion and is typically used when you want to load streaming data into 
  AWS data stores such as Amazon S3 or Amazon Redshift without having to manage the underlying infrastructure
- The primary purpose of Kinesis Data Firehose is to capture, transform, and load real-time streaming data
- To use Kinesis Data Firehose, you need to create a delivery stream, which represents the destination where the data 
  will be delivered
- Load large-scale streaming data into data lakes, data sources, and analytics services
- Firehose can ingest, process, and deliver streaming data to any number of endpoints and services
- This can include Amazon S3, Amazon Redshift, Amazon ElasticSearch Service, or generic HTTP endpoints, as well as 
  service providers
- It supports compression, batch processing, and can transform and encrypt data streams prior to loading, increasing  
  security, and reducing storage costs

# Data Analytics 
- This service allows you to run real-time analytics on streaming data
- You can use SQL-like queries to analyze the data as it flows through the Kinesis streams or Firehose
- It simplifies the process of gaining insights from real-time data without having to set up complex data processing pipelines
- It is commonly used for various real-time analytics scenarios, such as real-time monitoring, anomaly detection, fraud 
  detection, real-time reporting
- When using Kinesis Data Analytics, you typically define a Kinesis Data Analytics application, which consists of the 
  SQL queries, input data streams, and output data streams. The application continuously processes the incoming data and 
  stores the results in the specified output destinations

# Video Streams 
- It allows users to securely stream and store video data
- Kinesis Video Streams provides APIs for playback, allowing you to retrieve and replay video streams as needed
- You can use it to watch your video streams in real time as they are received in the cloud