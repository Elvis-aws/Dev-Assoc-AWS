
# File System Access
- You control which EC2 instances can access your EFS file system by using VPC security group rules and AWS Identity and 
  Access Management (IAM) policies
- Use VPC security groups to control the network traffic to and from your file system
- Attach an IAM policy to your file system to control which clients can mount your file system and with what permissions 
- Use EFS Access Points to manage application access
- Control access to files and directories with POSIX-compliant user and group-level permissions 
- Files and directories in an Amazon EFS file system support standard Unix-style read, write, and execute permissions 
  based on the user ID and group IDs
- When an NFS client mounts an EFS file system without using an access point, the user ID and group ID provided by the 
  client is trusted
- You can also use EFS access points to override user ID and group IDs used by the NFS client
- When users attempt to access files and directories, Amazon EFS checks their user IDs and group IDs to verify that each 
  user has permission to access the objects