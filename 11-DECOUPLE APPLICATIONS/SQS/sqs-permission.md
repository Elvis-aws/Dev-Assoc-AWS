
# Using Amazon SQS and IAM policies
- There are two ways to give your users permissions to your Amazon SQS resources
- Using the Amazon SQS policy system and using the IAM policy system 
- The IAM policy grants the rights to the Amazon SQS ReceiveMessage and SendMessage actions for the queue called 
  queue_xyz in your AWS Account, and the policy is attached to users named Bob and Susan (Bob and Susan have the 
  permissions stated in the policy)
- This Amazon SQS policy also gives Bob and Susan rights to the ReceiveMessage and SendMessage actions for the same queue
- There is one major difference between IAM and Amazon SQS policies: the Amazon SQS policy system lets you grant 
  permission to other AWS Accounts, whereas IAM doesn't