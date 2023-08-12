
# Visibility Timeout
- Visibility timeout is a period during which Amazon SQS prevents other consumers from receiving and processing a given 
  message
- The default visibility timeout for a message is 30 seconds
- The minimum is 0 seconds
- The maximum is 12 hours
- You cannot use visibility timeout to postpone the delivery of new messages to the queue for a few seconds