
# Vault Lock Policies
- An Amazon S3 Glacier (S3 Glacier) vault can have one resource-based vault access policy and one Vault Lock policy 
  attached to it
- A Vault Lock policy is a vault access policy that you can lock. 
- Using a Vault Lock policy can help you enforce regulatory and compliance requirements
- You can tag specific resources
# Use case
- As an example of a Vault Lock policy, suppose that you are required to retain archives for one year before you can 
  delete them
- To implement this requirement, you can create a Vault Lock policy that denies users permissions to delete an archive 
  until the archive has existed for one year
- You can test this policy before locking it down
- After you lock the policy, the policy becomes immutable