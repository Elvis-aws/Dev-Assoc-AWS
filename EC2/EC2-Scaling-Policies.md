
# Auto Scaling
- Target tracking: This policy lets you specify a scaling metric and metric value that your autoscaling group should 
      maintain at all times. For example your scaling metric is the average CPU utilization of your EC2 autoscaling 
      instances, and that their average should always be 80%. When CloudWatch detects that the average CPU utilization 
      is beyond 80%, it will trigger your target tracking policy to scale out the autoscaling group to meet this target 
      utilization. Once everything is settled and the average CPU utilization has gone below 80%, another scale in action 
      will kick in and reduce the number of autoscaling instances in your autoscaling group
- Simple scaling: This relies on a metric as a basis for scaling. For example, you can set a CloudWatch alarm to have a 
      CPU Utilization threshold of 80%, and then set the scaling policy to add 20% more capacity to your Auto Scaling 
      group by launching new instances. Accordingly, you can also set a CloudWatch alarm to have a CPU utilization 
      threshold of 30%. When the threshold is met, the Auto Scaling group will remove 20% of its capacity by terminating 
      EC2 instances
- Step Scaling: This improves the features of simple scaling. Step scaling applies “step adjustments” which means you 
      can set multiple actions to vary the scaling depending on the size of the alarm breach. When a scaling event 
      happens on simple scaling, the policy must wait for the health checks to complete and the cooldown to expire 
      before responding to an additional alarm. This causes a delay in increasing capacity especially when there is a 
      sudden surge of traffic on your application. With step scaling, the policy can continue to respond to additional 
      alarms even in the middle of the scaling event.
- Example: In this example, the Auto Scaling group maintains its size when the CPU utilization is between 40% and 60%. 
      When the CPU utilization is greater than or equal to 60% but less than 70%, the Auto Scaling group increases its 
      capacity by an additional 10%. When the utilization is greater than 70%, another step in scaling is done and the 
      capacity is increased by an additional 30%. On the other hand, when the overall CPU utilization is less than or 
      equal to 40% but greater than 30%, the Auto Scaling group decreases the capacity by 10%. And if utilization further 
      dips below 30%, the Auto Scaling group removes 30% of the current capacity.