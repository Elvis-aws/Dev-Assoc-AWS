
# S3 Notification
- The Amazon S3 notification feature enables you to receive notifications when certain events happen in your bucket
- To enable notifications, you must first add a notification configuration that identifies the events you want Amazon 
  S3 to publish and the destinations where you want Amazon S3 to send the notifications
# Destinations where it can publish events:
    - Amazon Simple Notification Service (Amazon SNS) topic
    - Amazon Simple Queue Service (Amazon SQS) queue
    - AWS Lambda
- Currently, the Standard SQS queue is only allowed as an Amazon S3 event notification destination, whereas the FIFO SQS 
  queue is not allowed