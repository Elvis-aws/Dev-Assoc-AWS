
# Launch Configuration
- A launch configuration is an instance configuration template that an Auto Scaling group uses to launch EC2 instances
- When you create a launch configuration, you specify information for the instances such as:
   - The ID of the Amazon Machine Image (AMI)
   - The instance type
   - A key pair
   - One or more security groups
   - A block device mapping
- You cannot use a launch configuration to provision capacity across multiple instance types using both On-Demand 
  Instances and Spot Instances