
# AWS DynamoDB Autoscaling
- Reduces waste in provisioned read or write resources
- DynamoDB autoscaling uses a scaling policy in Application Auto Scaling.
- To configure autoscaling in DynamoDB, you set the minimum and maximum levels of read and write capacity in addition 
  to the target utilization percentage.
- Autoscaling uses Amazon CloudWatch to monitor a table’s read and write capacity metrics. To do so, it creates 
  CloudWatch alarms that track consumed capacity
- The upper threshold alarm is triggered when consumed reads or writes breach the target utilization percent for two 
  consecutive minutes. The lower threshold alarm is triggered after traffic falls below the target utilization minus 20 
  percent for 15 consecutive minutes
- When an alarm is triggered, CloudWatch initiates autoscaling activity, which checks the consumed capacity and updates 
  the provisioned capacity of the table