
# Target Tracking Scaling Policy
- Use a backlog per instance metric with the target value being the acceptable backlog per instance to maintain
- To calculate your backlog per instance, divide the ApproximateNumberOfMessages queue attribute by the number of 
  instances in the InService state for the Auto Scaling group. Then set a target value for the Acceptable backlog per 
  instance
# Example
- Let's say that the current ApproximateNumberOfMessages is 1500 and the fleet's running capacity is 10
- If the average processing time is 0.1 seconds for each message and the longest acceptable latency is 10 seconds, then 
  the acceptable backlog per instance is 10 / 0.1, which equals 100. 
- This means that 100 is the target value for your target tracking policy
- If the backlog per instance is currently at 150 (1500 / 10), your fleet scales out, and it scales out by five instances 
  to maintain proportion to the target value