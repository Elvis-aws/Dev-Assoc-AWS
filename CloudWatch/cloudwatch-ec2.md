
# EC2 Status
- Using Amazon CloudWatch alarm actions, you can create alarms that automatically stop, terminate, reboot, or recover 
  your EC2 instances
- You can use the stop or terminate actions to help you save money when you no longer need an instance to be running
- You can use the reboot and recover actions to automatically reboot those instances or recover them onto new hardware 
  if a system impairment occurs
- You can create an Amazon CloudWatch alarm that monitors an Amazon EC2 instance and automatically reboots the instance
- The reboot alarm action is recommended for Instance Health Check failures (as opposed to the recover alarm action, 
  which is suited for System Health Check failures)