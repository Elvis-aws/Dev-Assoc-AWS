
# Microservices
- Elastic Container Services are ideal to run Microservices
# Let’s first understand what is a microservice
- Enterprises are heading towards microservices architectures 
- Microservices architecture focus on building small focused microservices
# Advantages of microservices:
- Flexibility to innovate and build applications in different programming languages (Go, Java, Python, JavaScript, etc)
- However deployments become complex!
  - How can we have one way of deploying Go, Java, Python or JavaScript .. microservices? 
  - Enter containers!
# Docker
- You can create Docker images for each microservice
- Docker image contains everything a microservice needs to run:
  - Application Runtime (JDK or Python or NodeJS)
  - Application code 
  - Dependencies
- You can run these docker containers the same way on any infrastructure:
  - Your local machine
  - Corporate data center 
  - Cloud
# Docker - Advantages
# Let’s look at some of the advantages that Docker provides:
- Docker containers are light weight (compared to Virtual Machines)
- Docker provides isolation for containers 
- Docker is cloud neutral
# As we build more and more Docker images for our microservices, a new challenge emerges
- How do you manage 1000’s of containers belonging to multiple microservices?
  - Enter Container Orchestration!
# Container Orchestration
# Requirement : 
- I want 10 instances of Microservice A container, 15 instances of Microservice B container and ....
# Typical Features of Container Orchestrator:
- Auto Scaling - Scale containers based on demand 
- Service Discovery - Help microservices find one another 
- Load Balancer - Distribute load among multiple instances of a microservice 
- Self Healing - Do health checks and replace failing instances 
- Zero Downtime Deployments - Release new versions without downtime
# Container Orchestration Options
# Let’s look at the different options for container orchestration.
- Let’s start with the Cloud Neutral option Kubernetes.
  - AWS service - AWS Elastic Kubernetes Service (EKS)
- Note: EKS does not have a free tier
- AWS Specific options include
  - AWS Elastic Container Service (ECS)
  - AWS Fargate : Serverless version of AWS ECS