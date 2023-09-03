
# Hosted Zone
- A hosted zone is an Amazon Route 53 concept
- A hosted zone is analogous to a traditional DNS zone file; it represents a collection of records that can be managed 
  together, belonging to a single parent domain name
- We have private or internal and public hosted zones
# Enable DNS Hostname
- DNS hostnames and DNS resolution are required settings for private hosted zones
- They are disabled by default and must be enabled
- DNS queries (DNS resolution) for private hosted zones can be resolved by the Amazon-provided VPC DNS server only
- As a result, these options must be enabled for your private hosted zone to work