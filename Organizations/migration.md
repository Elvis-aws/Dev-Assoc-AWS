
# Organizations
- AWS Organizations helps you centrally govern your environment as you grow and scale your workloads on AWS
- Using AWS Organizations, you can automate account creation, create groups of accounts to reflect your business needs, 
  and apply policies for these groups for governance
- You can also simplify billing by setting up a single payment method for all of your AWS accounts
- Through integrations with other AWS services, you can use Organizations to define central configurations and resource 
  sharing across accounts in your organization
# Migrating AWS Accounts
- To migrate accounts from one organization to another, you must have root or IAM access to both the member and master 
  accounts
- Here are the steps to follow:
1. Remove the member account from the old organization 
2. Send an invite to the member account from the new Organization
3. Accept the invite to the new organization from the member account