
# Storage Auto-Scaling
- If your workload is unpredictable, you can enable storage autoscaling for an Amazon RDS DB instance
- With storage autoscaling enabled, when Amazon RDS detects that you are running out of free database space it automatically 
  scales up your storage
- Amazon RDS starts a storage modification for an autoscaling-enabled DB instance when these factors apply
1. Free available space is less than 10 percent of the allocated storage
2. The low-storage condition lasts at least five minutes 
3. At least six hours have passed since the last storage modification
- The maximum storage threshold is the limit that you set for autoscaling the DB instance
- You can't set the maximum storage threshold for autoscaling-enabled instances to a value greater than the maximum 
  allocated storage