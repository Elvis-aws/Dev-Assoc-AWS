
# Gateway Endpoint
- Endpoints are virtual or logical devices. They are horizontally scaled, redundant, and highly available VPC components
- They allow communication between instances in your VPC and services without imposing availability risks or bandwidth 
  constraints on your network traffic
- A VPC endpoint enables you to privately connect your VPC to supported AWS services and VPC endpoint services powered 
  by AWS PrivateLink without requiring an internet gateway, NAT device, VPN connection, or AWS Direct Connect connection
- Instances in your VPC do not require public IP addresses to communicate with resources in the service
- Traffic between your VPC and the other service does not leave the Amazon network
# Types
- There are two types of VPC endpoints:
- Interface endpoint: An interface endpoint is an elastic network interface with a private IP address from the IP 
  address range of your subnet that serves as an entry point for traffic destined to a supported service
- Gateway endpoint: A gateway endpoint is a gateway that you specify as a target for a route in your route table for 
  traffic destined to a supported AWS service
- The following AWS services are supported: Amazon S3 and DynamoDB
# Resource
https://www.youtube.com/watch?v=6QS9YFGu5WI