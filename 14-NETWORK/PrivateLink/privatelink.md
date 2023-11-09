
# Private Link
- AWS PrivateLink simplifies the security of data shared with cloud-based applications by eliminating the exposure of 
  data to the public Internet
- AWS PrivateLink provides private connectivity between VPCs, AWS services, and on-premises applications, securely on 
  the Amazon network
- Can be used to create VPN endpoints
- Private Link is leveraged to create a private connection between an application that is fronted by an NLB in an 
  account, and an Elastic Network Interface (ENI) in another account, without the need of VPC peering and allowing the 
  connections between the two to remain within the AWS network
# Components
- VPC endpoint on the aws side
- VPC endpoint service on grafana side
- There is a load balancer fronting ec2 instances on grafana side
- A vpc endpoint on the aws side
- Both VPC should be in the same region
- If not then create a vpc peering or tunnel
- 
# Video
- https://www.youtube.com/watch?v=0lreDtiLtwk