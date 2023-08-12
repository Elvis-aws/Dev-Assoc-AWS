
# VPC peering
- A VPC peering connection is a networking connection between two VPCs that enables you to route traffic between them 
  using private IPv4 addresses or IPv6 addresses
- Instances in either VPC can communicate with each other as if they are within the same network
- You can create a VPC peering connection between your VPCs, or with a VPC in another AWS account
- The VPCs can be in different regions (also known as an inter-region VPC peering connection)
- VPC peering connections will work, but won't efficiently scale if you add more accounts (you'll have to create many 
  connections)