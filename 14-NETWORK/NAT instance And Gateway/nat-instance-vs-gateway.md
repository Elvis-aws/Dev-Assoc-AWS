
# IG
- Internet Gateway (IGW) allows instances with public IPs to access the internet. NAT Gateway (NGW) allows instances 
  with no public IPs to access the internet
- Unlike NAT Gateway and Internet Gateway, a NAT Instance is not a special service offered by AWS. It is just a term for 
  when using an EC2 instance to perform NAT Gateway-like functionality. It is similar to hosting database software on an 
  EC2 instance rather than using Amazon RDS


# NAT Gateway
- Highly available and is implemented in each availability zone with redundancy
- Managed by AWS
- Choose an Elastic IP (EIP) address to associate with a NAT gateway at the time of creation
- Automatically selected from the subnet’s IP address range when we create the gateway
- Not associated with any security group
- Use the network ACL to control traffic to and from the subnet in which NAT gateway resides
# NAT Instance
- Managed by cloud user
- Use an Elastic IP address or the public IP address with a NAT instance. We can change the public IP address at any 
  time by associating a new elastic IP address with the instance
- Assign a specific private IP address from the subnet IP address range when we launch an instance
- Associated with security group to control the inbound and outbound traffic
- Use the network ACL to control traffic to and from the subnet in which NAT instance resides
- 