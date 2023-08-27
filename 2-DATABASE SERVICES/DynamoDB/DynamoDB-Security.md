
# DynamoDB Security
- Encryption in transit using SSL/TLS by default
- Does not support encryption in transit for DAX
- Supports sever-side encryption using AWS KMS
- Supports client side encryption
- Default rest encryption method is AES-256 algorythm
- Customer Master Keys for encryption
    - AWS Owned CMK (Defaults): Keys are owned and managed by AWs. No additional charges
    - AWS Managed:  Keys are stored in your AWS account and managed by AWs KMS. Additional charges apply
    - Customer Managed: Keys are stored in the customers account, owned and managed by the customer. Additional charges 
      apply
- Use IAM policies to manage access
# Encryption
- All DynamoDB tables are encrypted
- There is no option to enable or disable encryption for new or existing tables
- By default, all tables are encrypted under an AWS owned customer master key (CMK) in the DynamoDB service account
- However, you can select an option to encrypt some or all of your tables under a customer-managed CMK or the AWS managed 
  CMK for DynamoDB in your account