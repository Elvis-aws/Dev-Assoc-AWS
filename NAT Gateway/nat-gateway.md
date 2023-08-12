
# NAT Gateway
- You can use a network address translation (NAT) gateway to enable instances in a private subnet to connect to the 
  internet or other AWS services, but prevent the internet from initiating a connection with those instances
- To create a NAT gateway, you must specify the public subnet in which the NAT gateway should reside. You must also 
  specify an Elastic IP address to associate with the NAT gateway when you create it. The Elastic IP address cannot be 
  changed after you associate it with the NAT Gateway
- If you have resources in multiple Availability Zones and they share one NAT gateway, and if the NAT gateway’s 
  Availability Zone is down, resources in the other Availability Zones lose internet access. To create an Availability 
  Zone-independent architecture, create a NAT gateway in each Availability Zone and configure your routing to ensure 
  that resources use the NAT gateway in the same Availability Zone