
# Event-Notifications
- When life-cycle transitions an object, u can get a notification
- When life-cycle expires an object, u can get a notification
- This can help u change dynamodb table indexes due to expiry notification
- Companies like CNN can store data in Deep Archive that they do not need. Let's say they want to broadcast a news and
  show some old video. What they do is they make an expedited request on the video file and get a notification when its 
  in S3-Standard which will be available for instant access

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