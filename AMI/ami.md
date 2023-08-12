
# EC2 AMI
- This is a virtual machine template
- You can customize the instance and then save this updated configuration as a custom AMI
- After you create and register an AMI, you can use it to launch new instances
- You can copy an AMI within the same AWS Region or to different AWS Regions
- When you no longer require an AMI, you can deregister it

# Copy AMI
- Go to created instance and select action dropdown
- Fill out Name, Destination region and Encryption options
- You can copy any AMI that you own, EBS or instance store (S3) backed, and with any operating system
- The copy process will result in a separate and new AMI in the destination region which will have a unique AMI ID
# Copying
- You can copy an AMI within or across AWS Regions using the AWS Management Console, the AWS Command Line Interface or 
  SDKs, or the Amazon EC2 API, all of which support the CopyImage action
- You can copy both Amazon EBS-backed AMIs and instance-store-backed AMIs
- You can copy AMIs with encrypted snapshots and also change encryption status during the copy process
- Copying an AMI backed by an encrypted snapshot cannot result in an unencrypted target snapshot
- You can share an AMI with another AWS account. To copy an AMI that was shared with you from another account, the owner 
  of the source AMI must grant you read permissions for the storage that backs the AMI, either the associated EBS 
  snapshot (for an Amazon EBS-backed AMI) or an associated S3 bucket (for an instance store-backed AMI)