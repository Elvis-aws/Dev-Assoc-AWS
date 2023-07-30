
# Global Accelerator
- AWS Global Accelerator is a networking service that helps you improve the availability, performance, and security of 
  your public applications
- Global Accelerator provides two global static public IPs that act as a fixed entry point to your application endpoints, 
  such as Application Load Balancers, Network Load Balancers, Amazon Elastic Compute Cloud (EC2) instances, and elastic IPs
- Global Accelerator’s IP addresses serve as the frontend interface of your applications
- It optimizes the path to the application to keep packet loss, jitter, and latency consistently low
- It uses the AWS global network to optimize the path from users to applications, improving the performance of TCP and 
  UDP traffic
- It provides static IP addresses that provide a fixed entry point to your applications and eliminate the complexity of 
  managing specific IP addresses for different AWS Regions and Availability Zones
- You don’t need to make any client-facing changes or update DNS records as you modify or replace endpoints
- It automatically re-routes traffic to the nearest healthy available endpoint to mitigate endpoint failure (redirect 
  traffic to healthy endpoints in less than 1 minute)
- It supports Client Affinity which helps build stateful applications
- It integrates with AWS Shield Standard, which minimizes application downtime and latency from DDoS attacks by using 
  always-on network flow monitoring and automated in-line mitigation
# Global Accelerator routes traffic to optimal AWS endpoints based on:
- Endpoint health
- Client locations
- User-configured weights