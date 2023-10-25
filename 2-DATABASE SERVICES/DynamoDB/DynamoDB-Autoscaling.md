
# AWS DynamoDB Autoscaling
- Reduces waste in provisioned read or write resources
- DynamoDB autoscaling uses a scaling policy
- Autoscaling uses Amazon CloudWatch to monitor a table’s read and write capacity metrics
- When an alarm is triggered, CloudWatch initiates autoscaling activity
# Amazon DynamoDB auto scaling
- DynamoDB auto-scaling uses the AWS Application Auto Scaling service to dynamically adjust provisioned throughput 
  capacity on your behalf, in response to actual traffic patterns
- This enables a table or a global secondary index to increase its provisioned read and write capacity to handle sudden 
  increases in traffic, without throttling
- When the workload decreases, Application Auto Scaling decreases the throughput so that you don't pay for unused 
  provisioned capacity
# Enable auto scaling
- If you use the AWS Management Console to create a table or a global secondary index, DynamoDB auto-scaling is enabled 
  by default
- When you delete a table or global table replica then any associated scalable targets, scaling polices, or CloudWatch 
  alarms are not automatically deleted with it