
# EC2 AMI
- AMIs are stored in Amazon S3 (region specific)
- AMIs contain:
  - Root volume block storage (OS and applications)
  - Block device mappings for non-root volumes
- You can configure launch permissions on an AMI
  - Who can use the AMI? 
  - You can share your AMIs with other AWS accounts
- Best Practice: Backup upto date AMIs in multiple regions
  - Critical for Disaster Recovery
- After you create and register an AMI, you can use it to launch new instances
- When you no longer require an AMI, you can deregister it
# Copy AMI
- Go to created instance and select action dropdown
- Fill out Name, Destination region and Encryption options
- You can copy any AMI that you own, EBS or instance store (S3) backed, and with any operating system
- This will result in a new AMI in the destination region which will have a unique AMI ID
# Copying
- You can copy an AMI within or across AWS Regions using the Console, or Command Line
- You can copy both Amazon EBS-backed AMIs and instance-store-backed AMIs
- You can copy AMIs with encrypted snapshots and also change encryption status during the copy process
- Copying an AMI backed by an encrypted snapshot cannot result in an unencrypted target snapshot
- You can share an AMI with another AWS account. To copy an AMI that was shared with you from another account, the owner 
  of the source AMI must grant you read permissions for the storage that backs the AMI, either the associated EBS 
  snapshot (for an Amazon EBS-backed AMI) or an associated S3 bucket (for an instance store-backed AMI)