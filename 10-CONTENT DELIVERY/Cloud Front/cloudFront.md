
# Amazon CloudFront
- Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, 
  and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment
- To distribute content using CloudFront you need to create a CloudFront Distribution
# Important features:
- Serve users from the nearest edge location (based on user location)
- Source content can be from S3, EC2, ELB and External Websites
- If content is not available at the edge location, it is retrieved from the origin server and cached
- No minimum usage commitment
# Use Cases:
- Static web apps. Audio, video and software downloads
- Dynamic web apps
- Support media streaming with HTTP and RTMP
# Amazon CloudFront Integrates with:
- AWS Shield to protect from DDoS attacks
- AWS Web Application Firewall (WAF) to protect from SQL injection, cross-site scripting, etc
# Cost Benefits:
- Zero cost for data transfer between S3 and CloudFront
- Reduce compute workload for your EC2 instances
# Important configuration options:
- DNS domain name - example abc.cloudfront.com
- Origins - Where do you get content from? S3, EC2, ELB, External Website
- Cache-Control
  - By default objects expire after 24 hours
  - Customize min, max, default TTL in CloudFront distribution
  - (For file level customization) Use Cache-Control max-age and Expires headers in origin server
- You can configure CloudFront to only use HTTPS (or) use HTTP for certain objects
  - Default is to support both HTTP and HTTPS
  - You can configure CloudFront to redirect HTTP to HTTPS
# Cache Behaviors
- Cache Behaviors help you to configure different CloudFront behavior for different URL path patterns from same origin
- TTL
# Options to secure content include:
# Signed URLs
- Signed URLS are used for:
  - RTMP distribution
  - Application downloads (individual files) and
  - Situations where cookies are not supported
# Signed cookies using key pairs
- Signed Cookies are used when you have multiple files (You have a subscriber website)
- Signed Cookies do not need any change in application URLs
# Origin Access Identities(OAI)
  - Ensures that only CloudFront can access S3
  - Allow access to S3 only to a special CloudFront user
- Origin Access Identities(OAI) allow Only CloudFront to access content in S3
# Here is the bucket policy configuration:
{
    "Version": "2012-10-17",
    "Id": "PolicyForCloudFrontPrivateContent",
    "Statement": [
        {
            "Effect": "Allow",
            "Principal": {
                "AWS": 
                "arn:aws:iam::cloudfront:user/CloudFront Origin Access Identity YOUR_IDENTIFIER"
            },
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::mybucket/*"
        }
    ]
}

