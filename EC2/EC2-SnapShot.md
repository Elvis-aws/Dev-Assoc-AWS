
# Using AMIs or Amazon EBS snapshots for backups and restore
- You can take a snapshot of an existing EC2 instance
- After that, you can go to actions and create a volume from the snapshot
- You can create an AMI from the snapshot
- You can use this AMI to create a new instance
- You can’t use snapshots to launch a new instance
- If you experience data corruption or a volume failure, you can create a volume from a snapshot that you have taken 
  and replace the old volume