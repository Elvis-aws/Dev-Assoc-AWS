      
# Auto Scaling
- Target tracking:   
     - Lets you specify a scaling metric and metric value that your autoscaling group should maintain at all times
     - CPU utilization of your EC2 autoscaling instances, and that their average should always be 80%
     - When CloudWatch detects that the average CPU utilization is beyond 80%, it will trigger your target tracking policy
     - Maintain CPU Utilization at 70%
        - Modify current capacity based on a target value for a specific metric
- Simple scaling: 
     - Set a CloudWatch alarm to have a CPU Utilization threshold of 80%, and then set the scaling policy to add 20% more 
       capacity to your Auto Scaling group 
     - When the threshold is met, the Auto Scaling group will remove 20% of its capacity by terminating 
        EC2 instances
     - +5 if CPU utilization > 80% -3 if CPU utilization < 60%
        - Waits for cooldown period before triggering additional actions
- Step Scaling: 
     - This improves the features of simple scaling. Step scaling applies “step adjustments” which means you 
        can set multiple actions to vary the scaling depending on the size of the alarm breach
     - +1 if CPU utilization between 70% and 80% +3 if CPU utilization between 80% and 100% Similar settings for scale down
         - Warm up time can be configured for each instance
# Cooldown period
- It allows you to temporally suspend scaling activity in other to allow the newly created instances to get configured
- if it takes an instance 400 seconds to be configured to receive traffic, and if the cooldown period is set lower than
  this value, a rise in configured metrix can trigger cloudwatch alarm to set of another scaling when the first has not
  yet been taken into effect
- It is a setting you can configure for your Auto Scaling group that helps to ensure that it doesn't launch or terminate 
  additional instances before the previous scaling activity takes effect
- A default cooldown period of 300 seconds is applied when you create your Auto Scaling group