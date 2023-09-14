
# Volume Gateway
- Volume Gateway : Move block storage to cloud
- Supports iSCSI protocol
- Reduce costs
- Automate backup and disaster recovery
- Use AWS Backup for backup and restore
- Use cases
  - Backup and disaster recovery
  - Migration of application data
- Cached (Gateway Cached Volumes):
  - Primary Data Store - AWS - Amazon S3
  - On-premise cache stores frequently accessed data
  - Data in S3 CANNOT be accessed directly
  - Take EBS snapshots from cached volumes
- Stored (Gateway Stored Volumes):
  - Primary Data Store - On-Premises
  - Asynchronous copy to AWS
  - Stored as EBS snapshots
    - For disaster recovery, restore to EBS volumes