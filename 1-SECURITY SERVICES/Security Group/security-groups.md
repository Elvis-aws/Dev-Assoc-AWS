
# AWS Security Groups
- An EC2 Security Groups is Virtual firewall to control incoming and outgoing traffic to/from AWS resources 
  (EC2 instances, databases etc)
- It Provides additional layer of security - Defense in Depth
- How are Security Group Rules evaluated?
  - Security groups are default deny. If there are no rules configured, no outbound/inbound traffic is allowed
  - You can specify allow rules ONLY
  - You can configure separate rules for inbound and outbound traffic
- You can assign multiple (up-to five) security groups to your EC2 instances
- You can add and delete security groups to EC2 instances at any time. Changes are immediately effective
- Traffic NOT explicitly allowed by Security Group will not reach the EC2 instance
- Security Groups are stateful:
  - If an outgoing request is allowed, the incoming response for it is automatically allowed
  - If an incoming request is allowed, an outgoing response for it is automatically allowed