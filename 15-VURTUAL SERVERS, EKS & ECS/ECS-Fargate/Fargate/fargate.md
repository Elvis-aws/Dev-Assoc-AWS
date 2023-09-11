
# AWS Fargate
- AWS Fargate is a technology that you can use with Amazon ECS to run containers without having to manage servers or 
  clusters of Amazon EC2 instances
- With Fargate, you no longer have to provision, configure, or scale clusters of virtual machines to run containers
- This removes the need to choose server types, decide when to scale your clusters, or optimize cluster packing
- When you run your Amazon ECS tasks and services with the Fargate launch type or a Fargate capacity provider, you 
  package your application in containers, specify the Operating System, CPU and memory requirements, define networking 
  and IAM policies, and launch the application
- Each Fargate task has its own isolation boundary and does not share the underlying kernel, CPU resources, memory 
  resources, or elastic network interface with another task
# When do you use these services to run Docker Containers in AWS?
- Elastic Beanstalk
  - Single container or multiple containers in same EC2 instance 
  - Recommended for simple web applications
- Amazon ECS
  - AWS specific solution for container orchestration 
  - Ideal for microservices
- Amazon Fargate
  - Serverless version of Amazon ECS 
  - You want to run microservices, and you don’t want to manage the cluster
- Amazon EKS
  - AWS managed service for Kubernetes 
  - Recommended if you are already using Kubernetes and would want to move the workload to AWS