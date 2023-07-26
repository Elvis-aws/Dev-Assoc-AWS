
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