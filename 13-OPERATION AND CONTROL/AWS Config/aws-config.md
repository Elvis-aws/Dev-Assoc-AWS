
# AWS Config
- AWS Config
  - What did my AWS resource look like?
- Auditing
  - Create a complete inventory of your AWS resources
- Resource history and change tracking
  - Find how a resource was configured at any point in time 
  - Configuration of deleted resources would be maintained 
  - Delivers history file to S3 bucket every 6 hours 
  - Take configuration snapshots when needed
- Governance
  - Customize Config Rules for specific resources or for entire AWS account 
  - Continuously evaluate compliance against desired configuration 
  - Get an SNS notification for every configuration change
- Consistent rules and compliance across AWS accounts:
  - Group Config Rules and Remediation Actions into Conformance Packs