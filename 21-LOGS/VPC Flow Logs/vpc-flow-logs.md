
# VPC Flow Logs
- VPC Flow Logs are used to Monitor network traffic
- Using VPC Flow Logs you can
    - Troubleshoot connectivity issues (NACL and/or security groups misconfiguration)
    - Capture traffic going in and out of your VPC (network interfaces)
- VPC Flow Logs can be created for
  - a VPC 
  - a subnet 
  - or a network interface (connecting to ELB, RDS, ElastiCache, Redshift etc)
- You can Publish logs to Amazon CloudWatch Logs or Amazon S3
- Flow log records contain ACCEPT or REJECT - Is the traffic permitted by security groups or network ACLs?
# Troubleshoot using VPC Flow Logs
- How do you troubleshoot issues? Here is some simplified logic:
    - Problem with response => Problem with NACL 
    - Problem with request could be problems with NACL or SG
- Inbound traffic rules are checked in this order: NACL IN, SG IN, NACL OUT (SG OUT NOT checked):
    - If inbound request is rejected, SG or NACL could be mis-configured 
    - If outbound response is rejected, NACL is mis-configured
- Outbound traffic rules are checked in this order: SG OUT, NACL OUT, NACL IN (SG IN NOT checked):
    - If outbound request is rejected, SG or NACL could be mis-configured 
    - If inbound response is rejected, NACL is mis-configured