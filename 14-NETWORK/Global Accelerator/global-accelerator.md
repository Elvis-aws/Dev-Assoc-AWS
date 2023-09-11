
# Global Accelerator
- Request going through many networks and hubs reducing latency
- Global accelerator reduces this inefficiency by using AWS Network
- It helps you improve the availability and performance of the applications that you offer to your global users
- It uses Anycast IP thus request from the edge location are routed to the nearest server
  - Unicast: One server holds one IP address
  - Anycast: Multiple server to hold the same IP address thus route to the nearest one
- It can forward requests to the following
  - Elastic IP
  - ALB
  - NLB
  - EC2 Instances
- It helps in disaster recover using health-checks: It regularly checks your endpoint and when its unhealthy, it 
  re-directs traffic to the healthy one
- Uses AWS shield for protection
# Used cases
- Single Region applications
- Multi Region applications
- Multi region storage
- Real time communication
- Gaming
# Video
- https://www.youtube.com/watch?v=jJUvamJgOqg