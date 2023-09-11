
# Questions
- You want to identify all instances belonging to a project, to an environment or to a specific billing type	
  - Add Tags. Project - A. Environment - Dev
- You want to change instance type	
  - Stop the instance
  - Use “Change Instance Type” to change and restart
- You don’t want an EC2 instance to be automatically terminated	
  - Turn on Termination Protection
  - (Remember) EC2 Termination Protection is not effective for terminations from 
    - a) Auto Scaling Groups (ASG) 
    - b) Spot Instances 
    - c) OS Shutdown
- You want to update the EC2 instance to a new AMI updated with latest patches	
  - Relaunch a new instance with an updated AMI
- Create EC2 instances based on on-premise Virtual Machine (VM) images	
  - Use VM Import/Export
  - You are responsible for licenses
- Change security group on an EC2 instance	
  - Assign at launch or runtime
  - Security Group changes are immediately effective
- You get a timeout while accessing an EC2 instance	
  - Check your Security Group configuration
- You are installing a lot of software using user data slowing down instance launch. How to make it faster?	
  - Create an AMI from the EC2 instance and use it for launching new instances
- I’ve stopped my EC2 instance. Will I be billed for it?	
  ZERO charge for a stopped instance (If you have storage attached, you have to pay for storage)