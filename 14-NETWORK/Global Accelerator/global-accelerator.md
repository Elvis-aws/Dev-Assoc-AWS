
# Global Accelerator
- User request from any point in the globe to an app on an EC2 instance goes through many networks and hubs
- This increases network latency and risk, because the request is going through the internet
- GA uses aws private network thus reducing the risk and latency
- It uses aws edge locations which will intend forward the request to the app
- It helps you improve the availability and performance of the applications
- It uses Anycast IP thus request from the edge location are routed to the nearest server
  - Unicast: One server holds one IP address
  - Anycast: Multiple server to hold the same IP address thus route to the nearest one
    - This static IP address provides a fixed entry point to your applications. This lets you easily move your end-points
      between AWS Regions without updating your DNS configuration
- It uses IPv4 addresses
- It can forward requests to the following
  - Elastic IP
  - ALB
  - NLB
  - EC2 Instances
- It helps in disaster recover using health-checks
- Uses AWS shield for protection
# Used cases
- A good fit for non-HTTP used cases such as
  - Gaming
  - IOT
  - Voice over
- Real time communication
# Video
- https://www.youtube.com/watch?v=jJUvamJgOqg