
# AWS DataSync
- Simple and fast to transfer data and files to AWS
- Automates process
- uses internet or Direct connect (VPC endpoint)
- Transfer rate is 10 Gbps
- Transfer files to the following destinations
  - Amazon EFS file system
  - Amazon FX for windows file system
  - Amazon S3
- Transfer between AWS regions
- Supports multiple destination
- Monitor progress using Amazon CloudWatch
# Use cases
- Data Migration, Data replication and Cold data archival
- Use AWS Snowball if you are bandwidth constrained or too much data
- Use S3 Transfer Acceleration when your applications are integrated with S3 API
- Migrate data using DataSync and use AWS Storage Gateway for ongoing updates from on-premises applications
# Process
- Configure datasync agent on-premise storage
- Create and connect agent in console
- Select service endpoint
- Choose security group
- Add agent IP address
- Create task
# Video
- https://www.youtube.com/watch?v=z3HKpLaAKhs