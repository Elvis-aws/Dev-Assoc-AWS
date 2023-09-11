
# AWS Network Access Control List
- Security groups control traffic to a specific resource in a subnet. How about stopping traffic from even entering the 
  subnet?
- NACL provides stateless firewall at subnet level
- Each subnet must be associated with a NACL
- Default NACL allows all inbound and outbound traffic
- Custom created NACL denies all inbound and outbound traffic by default
- NACL Rules have a priority number. Lower number => Higher priority
# Same subnet for EC2 instances and transit gateway association
- The same network ACL is used for both the traffic from the EC2 instances to the transit gateway and traffic from the 
  transit gateway to the instances
# NACL rules are applied as follows for traffic from instances to the transit gateway:
- Outbound rules use the destination IP address for evaluation
- Inbound rules use the source IP address for evaluation
# NACL rules are applied as follows for traffic from the transit gateway to the instances:
- Outbound rules are not evaluated
- Inbound rules are not evaluated
# Different subnets for EC2 instances and transit gateway association
- Consider a configuration where you have EC2 instances in one subnet and a transit gateway association in a different 
  subnet, and each subnet is associated with a different network ACL
# Network ACL rules are applied as follows for the EC2 instance subnet:
- Outbound rules use the destination IP address to evaluate traffic from the instances to the transit gateway
- Inbound rules use the source IP address to evaluate traffic from the transit gateway to the instances
# NACL rules are applied as follows for the transit gateway subnet:
- Outbound rules use the destination IP address to evaluate traffic from the transit gateway to the instances 
- Outbound rules are not used to evaluate traffic from the instances to the transit gateway 
- Inbound rules use the source IP address to evaluate traffic from the instances to the transit gateway
- Inbound rules are not used to evaluate traffic from the transit gateway to the instances
# Best Practices
Use a separate subnet for each transit gateway VPC attachment