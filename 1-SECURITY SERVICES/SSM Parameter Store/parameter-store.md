
# SSM Parameter Store
- AWS Systems Manager Parameter Store (aka SSM Parameter Store) provides secure, hierarchical storage for configuration 
  data management and secrets management
- You can store data such as passwords, database strings, EC2 instance IDs, Amazon Machine Image (AMI) IDs, and license 
  codes as parameter values
- You can store values as plain text or encrypted data
- You can reference Systems Manager parameters in your scripts, commands, SSM documents, and configuration and automation 
  workflows by using the unique name that you specified when you created the parameter
- SSM Parameter Store can serve as a secrets store, but you must rotate the secrets yourself, it doesn't have an automatic 
  rotation capability