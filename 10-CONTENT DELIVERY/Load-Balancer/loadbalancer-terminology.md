
# Elastic Load Balancer Terminology
- Connection draining - Before an instance is terminated, requests in execution are given time to complete 
  (deregistration_delay.timeout_seconds)
- Dynamic Host Port Mapping - Useful with containers. Two instances of the same task can be running on the same ECS 
  container instance
- Cross-zone load balancing - Distribute load between available instances in multiple AZs in One Region
- Sticky sessions - Send requests from same user to same instance (cookies with configurable expiration - Stickiness 
  duration default - 1 day)
- Preserve Source IP address - Allows instances to know where the request is coming from
- WebSockets - Allows full-duplex communication over a single TCP connection
- Source IP range (CIDR) based routing - Redirect to different targets based on the Source CIDR block
- Path(Route) Based Routing - Send traffic to different targets based on the path of the request
- Query string parameter-based routing - /user?target=target1 vs /user?target=target2
- Server Name Indication (SNI) - Support multiple websites with different SSL certificates with one Load Balancer