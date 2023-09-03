
# EC2 - Instance Metadata Service and Dynamic Data
- EC2 provides two important services to get details about an EC2 instance from within an EC2 instance
# Instance Metadata Service
- Instance Metadata Service helps you get details about EC2 instance from inside an EC2 instance
- Some of the important details include AMI ID, storage devices, DNS hostname, instance id, instance type, security 
  groups, IP addresses etc
- URL: http://169.254.169.254/latest/meta-data/
- Some of the important URL Paths include network, ami-id, hostname, local-hostname, local-ipv4 , public-hostname, 
  public-ipv4, security-groups, placement/availability-zone
# Dynamic Data Service:
- Dynamic Data Service helps you get dynamic information about EC2 instance
- URL: http://169.254.169.254/latest/dynamic/
- Example: http://169.254.169.254/latest/dynamic/instance-identity/document