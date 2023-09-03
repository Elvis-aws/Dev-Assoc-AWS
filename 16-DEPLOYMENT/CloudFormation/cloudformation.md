
# AWS CloudFormation
- AWS CloudFormation is a free-to-use Infrastructure as a Service (i.e. Pay only for the resources) that helps developers 
  and businesses to easily create the AWS resources and provision them in an orderly and predictable way
  - Provides a common language to describe and provision the AWS resources required for your infrastructure 
  - The configuration is defined in the simple JSON or YML file 
  - Understand the cloud dependencies i.e. It will first create a VPC, then subnets and later the resources in that subnet 
  - Offers functionality like -
    - Automatic rollback on errors 
    - Version control the configuration file
# Concepts
- Templates
  - The JSON or the YAML file that consists of the instructions for building the AWS resources in the cloud environment
    Developers can also use the CloudFromation Designer tool for creating, viewing, or modifying the 
    templates
- Stacks
  - Stack is a single unit describe by the Template and is created, updated, and deleted as when required. If 
    the resource creation gets failed, CloudFormation automatically rolls back the Stack and deletes the created 
    resources If the resource cannot be deleted, it is retained until the stack can be deleted successfully
- Stack sets
  - Allows to roll out the CloudFormation stacks over the multiple AWS accounts and in multiple regions with just a few 
    clicks. We can also specify the key and value pairs (popularly called as tags) during the Stack set create and update 
    operations
- Change Set
  - It is a summary of the changes that are proposed to the Stack and will allow the users to verify the impact that will 
    be propagated to the existing cloud environment
# Monitoring
- Since AWS provides effective monitoring for almost each of their services so in here we have the AWS CloudTrail (CT) 
  which provides a detail of the action taken by a user, role, or an AWS service
- CT captures the API calls for CloudFormation service as events
- Logs in Cloudwatch logs
# Security
- CloudFormation activities such as Create Stack, View Stack templates, or delete stacks can be controlled through IAM
- CloudFormation can use the IAM service role to make calls to the resources in a stack on your behalf
# Limits
- Resources = 200
- stack = 200
- StackSets = 100
- Stack instances per Stack set = 200