
# ECS Components
- Clusters
- Task definitions
- Tasks
- Services
- Containers and images
- Container agents

# Amazon ECS Launch Types
- The launch types are responsible for managing the compute resources
# EC2 Launch Type
- EC2 launch type allows more control but requires more management
- You still need to specify the underlying infrastructure details
- Your bill is based on the cost of the underlying EC2 instances
# Fargate Launch Type
- Service for running containerized application workloads
- Creating, configuring, and scaling clusters; or container host is managed by AWS
- You have to specify which operating system to use, the CPU and memory capacity needed
- You pay for the virtual CPU and memory resources that are consumed in running your tasks