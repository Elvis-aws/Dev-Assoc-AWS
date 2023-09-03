
# AWS CloudTrail
- Track events, API calls, changes made to your AWS resources:
  - Who made the request? 
  - What action was performed? 
  - What are the parameters used? 
  - What was the end result?
- (USE CASE) Compliance with regulatory standards
- (USE CASE) Troubleshooting. Locate a missing resource
- Delivers log files to S3 and/or Amazon cloud watch logs log group ( S3 is default )
- You can setup SNS notifications for log file delivery
- Log files are automatically encrypted with Amazon S3 SSE
- You can configure S3 Lifecycle rules to archive or delete log files
- Supports log file integrity
- You can prove that a log file has not been altered
