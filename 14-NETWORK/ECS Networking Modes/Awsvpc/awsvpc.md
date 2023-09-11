
# Awsvpc
- The awsvpc mode provides an elastic network interface for each task definition
- If you have one container per task definition, each container will have its own elastic network interface and will 
  get its own IP address from your VPC subnet IP address pool
- This offers faster performance than the bridge network since it uses the EC2 network stack, too
- This essentially makes each task act like their own EC2 instance within the VPC with their own ENI, even though the 
  tasks actually reside on an EC2 host 
- Awsvpc mode is recommended if your cluster will contain several tasks and containers as each can communicate with their 
  own network interface
- This is the only supported mode by the ECS Fargate service
- Since you don’t manage any EC2 hosts on ECS Fargate, you can only use awsvpc network mode so that each task gets its 
  own network interface and IP address