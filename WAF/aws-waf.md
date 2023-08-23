
# AWS WAF
- WAF is a web application firewall that helps protect web applications from attacks by allowing you to configure rules 
  that allow, block, or monitor (count) web requests based on conditions that you define
- These conditions include IP addresses, HTTP headers, HTTP body, URI strings, SQL injection and cross-site scripting
# How does AWS WAF block or allow traffic?
- As the underlying service receives requests for your web sites, it forwards those requests to AWS WAF for inspection 
  against your rules
- Once a request meets a condition defined in your rules, AWS WAF instructs the underlying service to either block or 
  allow the request based on the action you define
# How does AWS WAF protect my web site or application?
- WAF is tightly integrated with Amazon CloudFront, the Application Load Balancer (ALB), Amazon API Gateway, and AWS 
  AppSync – services that AWS customers commonly use to deliver content for their websites and applications
- When you use AWS WAF on Amazon CloudFront, your rules run in all AWS Edge Locations, located around the world close to 
  your end users
- This means security doesn’t come at the expense of performance
- Blocked requests are stopped before they reach your web servers
- When you use AWS WAF on regional services, such as Application Load Balancer, Amazon API Gateway, and AWS AppSync, 
  your rules run in region and can be used to protect internet-facing resources
# Deployment
- AWS WAF can be deployed on Amazon CloudFront
- AWS WAF can be deployed on Application Load Balancer (ALB)
- AWS WAF can be deployed on Amazon API Gateway
- AWS WAF can't be directly associated with an Amazon EC2 instance. Instead, register your Amazon EC2 instances as a 
  target for your Application Load Balancer (ALB) and then associate AWS WAF with the ALB