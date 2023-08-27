
# File Gateway
- Problem Statement: Large on-premise file share with terabytes of data
  - Users put files into file share and applications use the files
  - Managing it is becoming expensive
  - Move the file share to cloud without performance impact
- AWS Storage File Gateway provides cloud storage for your file shares
  - Files stored in Amazon S3 & Glacier
  - Supports Network File System (NFS) and Server Message Block (SMB)
- File gateway deployed as virtual machine on-premises
  - Maintains a local cache with most recently used objects
- Benefits from S3 features
  - High durability, low-cost, lifecycle management and cross-region replication
- Benefits from S3 integrations
  - Data analytics and machine learning applications using Amazon EMR or Amazon Athena
- Each file gateway supports up to 10 bucket shares