
# AWS Network Access Control List
- Security groups control traffic to a specific resource in a subnet. How about stopping traffic from even entering the 
  subnet?
- NACL provides stateless firewall at subnet level
- Each subnet must be associated with a NACL
- Default NACL allows all inbound and outbound traffic
- Custom created NACL denies all inbound and outbound traffic by default
- NACL Rules have a priority number. Lower number => Higher priority