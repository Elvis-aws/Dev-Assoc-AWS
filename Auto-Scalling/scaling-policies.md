      
# Auto Scaling
- Target tracking:   
     - Lets you specify a scaling metric and metric value that your autoscaling group should maintain at all times
     - CPU utilization of your EC2 autoscaling instances, and that their average should always be 80%
     - When CloudWatch detects that the average CPU utilization is beyond 80%, it will trigger your target tracking policy
- Simple scaling: 
     - Set a CloudWatch alarm to have a CPU Utilization threshold of 80%, and then set the scaling policy to add 20% more 
       capacity to your Auto Scaling group 
     - When the threshold is met, the Auto Scaling group will remove 20% of its capacity by terminating 
        EC2 instances
- Step Scaling: 
     - This improves the features of simple scaling. Step scaling applies “step adjustments” which means you 
        can set multiple actions to vary the scaling depending on the size of the alarm breach