
# AWS WAF
- WAF is a web application firewall that helps protect web applications from attacks by allowing you to configure rules 
  that allow, block, or monitor (count) web requests based on conditions that you define
- These conditions include IP addresses, HTTP headers, HTTP body, URI strings, SQL injection and cross-site scripting
# How does AWS WAF block or allow traffic?
- As the underlying service receives requests for your web sites, it forwards those requests to AWS WAF for inspection 
  against your rules
- Once a request meets a condition defined in your rules, AWS WAF instructs the underlying service to either block or 
  allow the request based on the action you define
# Deployment
- Can only be deployed on content serving services such as Amazon CloudFront, Application Load Balancer, API Gateway
- AWS WAF can't be directly associated with an Amazon EC2 instance
# WACL
- A web access control list (web ACL) gives you fine-grained control over all of the HTTP(S) web requests that your 
  protected resource responds to. You can protect Amazon CloudFront, Amazon API Gateway, Application Load Balancer, 
  AWS AppSync, Amazon Cognito, AWS App Runner, and AWS Verified Access resources
- There are managed and owned rules