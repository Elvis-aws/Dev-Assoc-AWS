
# ALB
- Use cases
  - Web apps, microservices & containers
- Protocols Supported
  - HTTP, HTTPS (Layer 7)
- Connection draining: Yes
- Dynamic Host Port Mapping: Yes
- Server Name Indication (SNI): Yes
- WebSockets: Yes
- IP addresses as targets: Yes
- Source IP address range (CIDR) based routing: Yes
- Path(Route) Based Routing: Yes
- Host-Based Routing: Yes
- Fixed response: Yes
- Lambda functions as targets: Yes
- HTTP header-based routing: Yes
- HTTP method-based routing: Yes
- Query string parameter-based routing
# Network LB
- Use cases
  - Extreme performance - millions of requests with less latency (100ms)
- Protocols Supported
  - TCP, UDP, TLS (Layer 4)
- Dynamic Host Port Mapping: Yes
- Server Name Indication (SNI): Yes
- Static IP: Yes
- Elastic IP address: Yes
- Preserve Source IP address: Yes
- WebSockets: Yes
- IP addresses as targets: Yes
# Classic Load Balancer
- Use cases
  - Avoid if possible. Not recommended by AWS
- Protocols Supported
  - TCP, SSL/TLS, HTTP, HTTPS(Layer 4 & 7)
- Connection draining: Yes

# Few important things to note:
- Elastic Load Balancer is a Managed service
- AWS ensures that it is highly available
- ELB Auto scales to handle huge loads
- Load Balancers can be public or private
- We can configure Health checks to route traffic to healthy instances

# Listeners
- Each Load Balancer has one or more listeners listening for connection requests from the client
- Each listener has:
  - a protocol
  - a port
  - a set of rules to route requests to targets

# Listener Rules
- How do I identify which request should be sent to which target group?
  - Configure multiple listener rules for the same listener

# Target Groups
- How to group instances that ALB has to distribute the load between?
- Create a Target Group
  - A target group can be:
- A set of EC2 instances
- A lambda function
- Or a set of IP addresses

# Target Group Configuration - Sticky Session
- Enabling sticky user sessions sends all requests from one user to the same instance.
- Important things to note:
  - Implemented using a cookie
  - Supported by ALB and CLB

# Load Balancer Health Checks
- Give warm up time to EC2 instances before they start receiving load from ELB
  - Configure Health Check Grace Period

# Elastic Load Balancer - Debugging and Tracing - Logs and Headers
- You can enable access logs on ELB to capture:
  - Time request was received
  - Client’s IP address
  - Latencies
  - Request Paths, and
  - Server Response
- Network Load Balancer allows the EC2 instance to see the client request details directly. HOWEVER, Application Load 
  Balancer does NOT. In Application Load Balancer, Client details are passed in request headers:
  - X-Forwarded-For: Client IP address
  - X-Forwarded-Proto: Originating Protocol - HTTP/HTTPS
  - X-Forwarded-Port: Originating Port