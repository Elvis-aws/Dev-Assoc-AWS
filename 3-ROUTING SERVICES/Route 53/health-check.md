
# Health Check
- You can use Route 53 health checking to configure active-active and active-passive failover configurations
# Active-active failover
- Use this failover configuration when you want all of your resources to be available the majority of the time
- When a resource becomes unavailable, Route 53 can detect that it's unhealthy and stop including it when responding to 
  queries 
- In active-active failover, all the records that have the same name, the same type (such as A or AAAA), and the same 
  routing policy (such as weighted or latency) are active unless Route 53 considers them unhealthy
- Route 53 can respond to a DNS query using any healthy record
# Active-passive failover
- Use an active-passive failover configuration when you want a primary resource or group of resources to be available 
  the majority of the time and you want a secondary resource or group of resources to be on standby in case all the 
  primary resources become unavailable
- When responding to queries, Route 53 includes only the healthy primary resources
- If all the primary resources are unhealthy, Route 53 begins to include only the healthy secondary resources in response 
  to DNS queries
# Configure active-passive failover 
- Create a health check for each resource that you want to route traffic to, such as an EC2 instance or a web server in 
  your data center
- Create records for your primary resources, and specify the following values:
  - Give each record the same name, type, and routing policy 
  - If you're using AWS resources that you can create alias records for, specify Yes for Evaluate Target Health
- Create records for your secondary resources, if applicable, and specify the following values:
  - Give each record the same name, type, and routing policy 
  - If you're using AWS resources that you can create alias records for, specify Yes for Evaluate Target Health
  - If you're using resources that you can't create alias records for, associate the applicable health check from step 
    1 with each record
- Create two failover alias records, one primary and one secondary, and specify the following values:
  - Set Failover Record Type – Specify Primary for primary record
  - Set Failover Record Type – Specify Secondary for secondary record
