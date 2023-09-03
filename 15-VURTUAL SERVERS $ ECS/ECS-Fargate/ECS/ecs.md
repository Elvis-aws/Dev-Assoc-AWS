
# Amazon Elastic Container Service (Amazon ECS)
- Amazon Elastic Container Service (Amazon ECS) is a fully managed service for container orchestration
- AWS Fargate is a serverless option 
# Use cases include:
- Microservices Architectures - Create containers for your microservices and orchestrate them using ECS or Fargate
- Batch Processing. Run batch workloads on ECS using AWS Batch
# Amazon ECS - Task Definition
- To manage containers using Amazon ECS, you need Tasks 
- Tasks contain Container Definition(s)
  - What is the image you want to use? 
  - What resources does the container use (memory, CPU and ports)?
# Two important task related configuration to remember:
- Task Role (Optional): If you need access to AWS services (Amazon RDS etc)
- Task execution IAM role: Provides permissions to pull container images and publish container logs to Amazon CloudWatch
# Amazon ECS - Terminology
- Here is the important terminology used in ECS
  - Service: Allows you to run and maintain a specified number (the “desired count”) of tasks 
  - ECS cluster: Grouping of one or more container instances (EC2 instances) where you run your tasks 
  - Container Instance - EC2 instance in the cluster running a container agent (helps it communicate with the cluster)
    - AWS provides ECS ready AMIs with container agents pre-installed
# Amazon Elastic Container Service - Remember
- AWS Fargate does NOT give you visibility into the EC2 instances in the cluster
- You can use On-Demand instances or Spot instances to create your cluster
- You can load balance using Application Load Balancers
  - Two features of ALB are important for ECS:
    - Dynamic host port mapping: Multiple tasks from the same service are allowed per EC2 (container) instance 
    - Path-based routing: Multiple services can use the same listener port on same ALB and be routed based on path 
      (www.app.com/microservice-a and www.app.com/microservice-b)