
#  Launch Template
- A launch template is similar to a launch configuration, in that it specifies instance configuration information such 
  as
   - The ID of the Amazon Machine Image (AMI)
   - The instance type
   - A key pair
   - Security groups, and the other parameters that you use to launch EC2 instances
- Also, defining a launch template instead of a launch configuration allows you to have multiple versions of a template
- With launch templates, you can provision capacity across multiple instance types using both On-Demand Instances and 
  Spot Instances to achieve the desired scale, performance, and cost