
# How GuardDuty Works
- Cloud Trail Event Logs
    - Unusual API calls
    - Un authorised deployments
- Cloud Trail Management Events
    - Create VPC events
    - Create Subnet events
- Cloud Trail S3 Data Events
    - Get objects
    - Delete objects
    - Put objects
- VPC Flow Logs
    - Unusual Internet Traffic
    - Unusual IP Addresses
- DNS Logs
    - Compromised EC2 Instances sending encoded data
- Kubernetes Audit Logs
    - Suspicious activities
    - EKS Cluster compromise
- Protect against Crypto Currency attack

# GuradDuty
- All these logs will go into GuardDuty
- Findings will be generated
- These findings will then trigger EventBridge rules
- These will then be sent to SNS for notification or Lambda
# Delete Data
- Disabling the service will delete all remaining data, including your findings and configurations before relinquishing 
  the service permissions and resetting the service
