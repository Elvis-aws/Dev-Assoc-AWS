
# Monitoring AWS with Amazon CloudWatch
- Monitoring and observability service
- Collects monitoring and operational data in the form of logs, metrics, and events
- Set alarms, visualize logs, take automated actions and troubleshoot issues
- Integrates with more than 70 AWS services:
  - Amazon EC2 
  - Amazon DynamoDB 
  - and ….
# Amazon CloudWatch Logs
- Monitor and troubleshoot using system, application and custom log files
- Real time application and system monitoring
  - Monitor for patterns in your logs and trigger alerts based on them 
  - Example : Errors in a specific interval exceed a certain threshold
- Long term log retention
  - Store logs in CloudWatch Logs for as long as you want (configurable - default:forever)
  - Or archive logs to S3 bucket (Typically involves a delay of 12 hours)
  - Or stream real time to Amazon Elasticsearch Service (Amazon ES) cluster using CloudWatch Logs subscription
# Agents
- CloudWatch Logs Agent
  - Installed on ec2 instances to move logs from servers to CloudWatch logs
- CloudWatch Logs Insights
  - Write queries and get actionable insights from your logs
- CloudWatch Container Insights
  - Monitor, troubleshoot, and set alarms for your containerized applications running in EKS, ECS and Fargate
# Alarm
- Create alarms based on:
  - Amazon EC2 instance CPU utilization 
  - Amazon SQS queue length 
  - Amazon DynamoDB table throughput or 
  - Your own custom metrics
# EC2 Status
- You can create alarms that automatically stop, terminate, reboot, or recover your EC2 instances