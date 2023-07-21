
# ECS Components
- Clusters
- Task definitions
- Tasks
- Services
- Containers and images
- Container agents

# Amazon ECS Launch Types
- Launch types, or instance launch types, are hardware environments based on the host computer where your application 
  is deployed. The launch types are responsible for managing the compute resources dedicated to deploying your application. 
  Amazon ECS supports two launch types for running containers, Amazon EC2 and AWS Fargate
# EC2 Launch Type
- EC2 launch type allows more control but requires more management. When using the EC2 launch type, you still need to 
  specify the underlying infrastructure details, the launch instance, the network security setting, and the auto-scaling 
  group if applicable
- When you use EC2 instances as capacity, it means your bill is based on the cost of the underlying EC2 instances
# Fargate Launch Type
- Fargate launch type is the serverless service for running containerized application workloads. You don’t need to worry 
  about the underlying infrastructure; creating, configuring, and scaling clusters; or container host. These configurations 
  are made and managed by AWS, but you have to specify which operating system to use, the CPU and memory capacity needed 
  to package your application, the network security setting, and IAM policies
- In terms of cost, you only have to pay for the virtual CPU and memory resources that are consumed in running your tasks