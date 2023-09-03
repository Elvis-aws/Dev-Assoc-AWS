
# REST API Challenges
- Most applications today are built around REST API
- Management of REST API is not easy:
  - You’ve to take care of authentication and authorization 
  - You’ve to be able to set limits (rate limiting, quotas) for your API consumers 
  - You’ve to take care of implementing multiple versions of your API 
  - You would want to monitor your API calls 
  - You would want to be able to cache API requests
# Amazon API Gateway
- How about a fully managed service with auto-scaling that can act as a “front door” to your APIs? Welcome 
  “Amazon API Gateway”
- Amazon API Gateway helps you to “publish, maintain, monitor, and secure APIs at any scale”
- You can authorize users by integrating with:
  - AWS IAM (for AWS users using signature version 4)
  - Amazon Cognito 
  - Lambda authorizer (custom authorization with JWT tokens or SAML)
# Amazon API Gateway Features
- Integrates with AWS Lambda, Amazon EC2, Amazon ECS or any web application
- Supports HTTP(S) and WebSockets (two way communication - chat apps and streaming dashboards)
- Serverless. Pay for use (API calls and connection duration)
- Provides API Lifecycle Management for RESTful APIs and WebSocket APIs
- You can Run multiple versions of the same API
- Supports Rate Limits(request quota limits), throttling and fine-grained access permissions using API Keys for 
  Third-Party Developers
- Lifecycle management for REST APIs
- Versioning and multiple environments
- API keys - Generate API keys to monitor usage
  - Implement plans and quota limits for external applications (or developer)
  - WARNING - Do NOT use API keys for Authorization
- Enable caching for API calls with TTL
- Protect backends by throttling requests
- Integrates with
  - Amazon CloudWatch - Performance metrics, API calls, latency data and error rates 
  - Amazon CloudWatch Logs - Debug logging 
  - AWS CloudTrail - Complete history of changes to your REST API