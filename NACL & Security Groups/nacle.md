
# NACLE
- It is an optional layer of security that acts as a firewall for controlling traffic in and out of a subnet
- You can associate multiple subnets with a single network ACL, but a subnet can be associated with only one network 
  ACL at a time
# Connectivity
- To enable the connection to a service running on an instance, the associated network ACL must allow both inbound traffic 
  on the port that the service is listening on as well as allow outbound traffic from ephemeral ports
- When a client connects to a server, a random port from the ephemeral port range (1024-65535) becomes the client's source 
  port
- The designated ephemeral port then becomes the destination port for return traffic from the service, so outbound traffic 
  from the ephemeral port must be allowed in the network ACL
- By default, network ACLs allow all inbound and outbound traffic
- If your network ACL is more restrictive, then you need to explicitly allow traffic from the ephemeral port range
- If you accept traffic from the internet, then you also must establish a route through an internet gateway
- If you accept traffic over VPN or AWS Direct Connect, then you must establish a route through a virtual private gateway