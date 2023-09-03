
# Standby
- You can put an instance that is in the InService state into the Standby state, update or troubleshoot the instance, and 
  then return the instance to service
- Instances that are on standby are still part of the Auto Scaling group, but they do not actively handle load balancer 
  traffic
- This feature helps you stop and start the instances or reboot them without worrying about Amazon EC2 Auto Scaling 
  terminating the instances as part of its health checks or during scale-in events
# DetachInstances
- You can now remove an instance from an Auto Scaling Group and manage it independently
- The instance can remain unattached, or you can attach it to another Auto Scaling Group if you’d like
- When you call the DetachInstances function, you can also request a change in the desired capacity for the group
- Detaching instances might be useful if you want to manage the instances like standalone EC2 instances and possibly 
  terminate them