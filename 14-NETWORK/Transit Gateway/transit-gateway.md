
# Transit Gateway
- Regular VPC peering connections are 1-1
- AWS Transit Gateway is a service that enables customers to connect their Amazon Virtual Private Clouds (VPCs) and 
  their on-premises networks to a single gateway
- You are charged hourly for each attachment on a transit gateway, and you are charged for the amount of traffic 
  processed on the transit gateway
- As your cloud infrastructure expands globally, inter-Region peering connects transit gateways together using the AWS 
  Global Infrastructure
- All network traffic between AWS data centers is automatically encrypted at the physical layer
# Regional Service
- As a regional resource with high availability, AWS Transit Gateway will be set up in two regions and connected by 
  inter-region peering
- AWS Transit Gateway Network Manager makes use of other AWS services, particularly Amazon CloudWatch and Amazon VPC Flow 
  Logs, to manage and monitor AWS-based networks