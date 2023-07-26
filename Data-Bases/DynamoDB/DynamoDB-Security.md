
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