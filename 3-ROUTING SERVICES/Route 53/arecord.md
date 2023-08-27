
# A Record
- A record (or Address record) value is always an IP address. The IP should be static i.e. it should not change frequently. 
  For example, Elastic IPs in AWS are static IPs
# Use Case:
- A record will be used to map your root/naked domain-name viz example.com  to  Elastic IP say 198.51.100.77. You can map 
  an IPv4 Public IP with A record. But it is not recommended as Public IP can change when you STOP & START an EC2 instance