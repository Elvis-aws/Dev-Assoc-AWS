
# Recover EC2 Instance
- If your instance fails a system status check, you can use CloudWatch alarm actions to automatically recover it
- The CloudWatch recovery option works only for system check failures, not for instance status check failures
- Also, if you terminate your instance, then it can't be recovered 
- You can create an Amazon CloudWatch alarm that monitors an Amazon EC2 instance and automatically recovers the instance 
  if it becomes impaired due to an underlying hardware failure or a problem that requires AWS involvement to repair
- Terminated instances cannot be recovered
- A recovered instance is identical to the original instance, including the instance ID, private IP addresses, Elastic 
  IP addresses, and all instance metadata
- If the impaired instance is in a placement group, the recovered instance runs in the placement group
- The automatic recovery process attempts to recover your instance for up to three separate failures per day
- Your instance may subsequently be retired if automatic recovery fails and a hardware degradation is determined to be 
  the root cause for the original system status check failure