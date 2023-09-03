
# AWS Organizations
- Organizations typically have multiple AWS accounts
  - Different business units
  - Different environments
- How do you centralize your management (billing, access control, compliance and security) across multiple AWS accounts?
- Welcome AWS Organizations!
- Organize accounts into Organizational Units (OU)
- Provides API to automate creation of new accounts
# AWS Organizations - Features
- One consolidated bill for all AWS accounts
- Centralized compliance management for AWS Config Rules
- Send AWS CloudTrail data to one S3 bucket (across accounts)
- AWS Firewall Manager to manage firewall rules (across accounts)
  - AWS WAF, AWS Shield Advanced protections and Security Groups
- Use Service control policies (SCPs) to define restrictions for actions (across accounts):
- Prevent users from disabling AWS Config or changing its rules
- Require Amazon EC2 instances to use a specific type
- Require MFA to stop an Amazon EC2 instance
- Require a tag upon resource creation
# AWS Service Quotas
- AWS account has Region-specific default quotas or limits for each service
- Service Quotas allows you to manage your quotas for over 100 AWS services, from one location