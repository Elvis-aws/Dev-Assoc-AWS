
# Guard Duty
- GuardDuty is an intelligent threat detection service that continuously monitors your AWS accounts, Amazon Elastic 
  Compute Cloud (EC2) instances, Amazon Elastic Kubernetes Service (EKS) clusters, and data stored in Amazon Simple 
  Storage Service (S3) for malicious activity without the use of security software or agents
- If potential malicious activity, such as anomalous behavior, credential ex-filtration, or command and control 
  infrastructure (C2) communication is detected, GuardDuty generates detailed security findings that can be used for 
  security visibility and assisting in remediation
- Additionally, using the Amazon GuardDuty Malware Protection feature helps to detect malicious files on Amazon Elastic 
  Block Store (EBS) volumes attached to EC2 instance and container workloads
# GuardDuty detects three main types of threats:
- Compromised instances: GuardDuty will detect any unusual spikes in network traffic, as well as hijacked resources 
  such as an external IP address hijacking EC2 instances
- Reconnaissance: Reconnaissance is when an attacker gathers information about the network. GuardDuty detects activity 
  that suggests reconnaissance, such as unblocked port probing from a known malicious IP, VPC port scanning, and unusual 
  API activity
- Compromised accounts: GuardDuty will detect common patterns that indicate an account compromise, such as API calls 
  from unusual locations, updates that weaken the account’s password policy and API calls from known malicious IPs