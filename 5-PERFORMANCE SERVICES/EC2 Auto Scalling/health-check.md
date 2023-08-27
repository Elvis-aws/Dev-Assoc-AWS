
# Health Check
- By default, health check grace period is set to 300 seconds, termination will not happen except the grace period has expired
- Amazon EC2 Auto Scaling does not immediately terminate instances with an Impaired status ( the instance is not running 
  or un-reachable). Instead, Amazon EC2 Auto Scaling waits a few minutes for the instance to recover
- Amazon EC2 Auto Scaling doesn't terminate instances that fail ELB health checks