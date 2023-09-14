
# AWS FSX File system
- Almost same as EFS
- Amazon FSx lets you easily and securely backup, archive, or replicate your on-premises file storage to AWS in order 
  to meet regulatory, data retention, or disaster recovery requirements.
- Amazon FSX for Lustre provides two file system deployment
    - Scratch: Temporary storage and short term data processing
    - Persistent: Persist and data replication
# Two flavours
- Amazon FSx for Windows File Server
  - For windows applications
  - You must have active directory
  - Build on SSD storage
  - Shared file system
  - Multi Az file system (Failover)
- Amazon FSx for Lustre (Linux)
  - High performance file system
  - Faster than EFS
  - Connects to S3 (Replicates data in S3)
  - Compatible with windows and Linux
  - 