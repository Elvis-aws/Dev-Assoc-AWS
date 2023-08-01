
# CMK
- Deleting a KMS key is destructive and potentially dangerous
- You should proceed only when you are sure that you don't need to use the KMS key anymore and won't need to use it in 
  the future
- If you are not sure, you should disable the KMS key instead of deleting it
- You have to define a waiting period in the scheduled deletion task.
- If you don’t define a waiting period, the period defaults to 30 days
- In this period, the deletion transitions to pending state
- Within this period, you can cancel deletion
- As an additional safety measure, you can create an Amazon CloudWatch alarm to alert you when a request on the key has 
  been made during the waiting period