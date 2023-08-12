
# Alias
- AWS Route 53 Alias record is a type of DNS record that allows you to map a hostname to a specific Amazon Web Services 
  (AWS) resource, such as an Amazon S3 bucket, an Elastic Load Balancer, or a CloudFront distribution 
- An Alias record works similarly to a CNAME record, in that it allows you to point a subdomain to another destination. 
  However, there are some key differences between Alias records and CNAME records
1. Alias records can be used to map a hostname to any AWS resource that has a publicly resolvable DNS name, whereas CNAME 
   records can only map to a domain or subdomain 
2. Alias records can be updated automatically if the IP address of the AWS resource changes, whereas CNAME records would 
   need to be updated manually
3. Alias records are free, unlike CNAME records, you don't have to pay for each Alias record

[https://www.youtube.com/watch?v=ZXCQwdVgDno](https://www.youtube.com/watch?v=ZXCQwdVgDno)