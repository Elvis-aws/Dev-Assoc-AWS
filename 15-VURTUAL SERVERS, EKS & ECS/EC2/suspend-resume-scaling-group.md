Consider the following before suspending processes:

# Suspend and Resume
- Suspending a process affects all instances in your Auto Scaling group. For example, you can suspend the HealthCheck 
  and ReplaceUnhealthy processes to reboot instances without Amazon EC2 Auto Scaling terminating the instances based on 
  its health checks. If you need Amazon EC2 Auto Scaling to perform health checks on remaining instances, then use the 
  standby feature instead of the suspend-resume feature. For more information, see Temporarily remove instances from 
  your Auto Scaling group
- Suspending AlarmNotification allows you to temporarily stop the group's target tracking, step, and simple scaling 
  policies without deleting the scaling policies or their associated CloudWatch alarms. To temporarily stop individual 
  scaling policies instead, see Disable a scaling policy for an Auto Scaling group
- If you suspend the Launch and Terminate processes, or AZRebalance, and then you make changes to your Auto Scaling 
  group, for example, by detaching instances or changing the Availability Zones that are specified, your group can become 
  unbalanced between Availability Zones. If that happens, after you resume the suspended processes, Amazon EC2 Auto 
  Scaling gradually redistributes instances evenly between the Availability Zones
- Suspending the Terminate process doesn't prevent the successful termination of instances using the force delete option 
  with the delete-auto-scaling-group command
- The RemoveFromLoadBalancerLowPriority process should be ignored when it is present in calls to describe Auto Scaling 
  groups using the AWS CLI or SDKs. This process is deprecated and is retained only for backward compatibility