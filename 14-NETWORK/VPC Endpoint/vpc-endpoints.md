
# VPC Endpoint
- VPC Endpoint helps you to securely connect your VPC to another service.
# There are two types
- Gateway endpoint
  - Help you to securely connect to Amazon S3 and DynamoDB 
  - Endpoint serves as a target in your route table for traffic 
  - Provide access to endpoint (endpoint, identity and resource policies)
  - Not accessible from on premise
- Interface endpoint
  - Help you to securely connect to AWS services EXCEPT FOR DynamoDB 
  - You can also access S3 through this endpoint
  - Accessible from on premise
  - Powered by PrivateLink (keeps network traffic within AWS network)
  - Needs an elastic network interface (ENI) (entry point for traffic)
# Important things to remember about VPC Endpoints:
- (Avoid DDoS & MTM attacks) Traffic does NOT go through internet
- (Simple) Does NOT need Internet Gateway, VPN or NAT
