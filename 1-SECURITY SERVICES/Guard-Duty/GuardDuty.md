
# Guard Duty
- Amazon GuardDuty is a threat detection service that continuously monitors for malicious activity and unauthorized 
  behavior to protect your AWS accounts, Amazon Elastic Compute Cloud (EC2) workloads, container applications, Amazon 
  Aurora databases, and data stored in Amazon Simple Storage Service (S3)
- Suspicious activity
# GuardDuty detects three main types of threats:
- Compromised instances: GuardDuty will detect any unusual spikes in network traffic
- Reconnaissance: Reconnaissance is when an attacker gathers information about the network
- Compromised accounts: GuardDuty will detect common patterns that indicate an account compromise
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
- Disabling the service will delete all remaining data
# Video
- https://www.youtube.com/watch?v=4rR37ZBJWdI
# Threat 
- Something that can damage asset or steal data