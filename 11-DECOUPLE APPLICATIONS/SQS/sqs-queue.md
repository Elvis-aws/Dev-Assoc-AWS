
# SQS
- Amazon SQS is a fully managed service popular for its message queuing functionality
- Developers often send and retrieve messages of various types and sizes asynchronously using this service
- Messages can contain up to 256 KB of text in any format such as json, xml, etc
- Messages are kept in a queue from 1 minute to 14 days
- The default retention period is 4 days
- It guarantees that your messages will be processed at least once
- There are two types, FIFO and Standard

# Batch size
- Batch size effects how many SQS messages can be included in a single event
- The default batchSize is 10. The max batchSize is 10000 for a standard queue, 10 for a FIFO queue
- You can also set maximumBatchingWindow to standard queues to specify the maximum amount of time in seconds to gather 
  records before invoking the function. The max maximumBatchingWindow is 300 seconds
- FIFO queues support 300 messages per second
- When you can batch 10 messages per operation, they can support 3000 messages per second

# Group ID
- If we don't specify a GroupID, then all the messages are in absolute order, but we can only have 1 consumer at most
- To allow for multiple consumers to read data and to scale the number of consumers, we should use the "Group ID" attribute