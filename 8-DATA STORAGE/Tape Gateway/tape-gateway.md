
# Tape Gateway
- Tape backups used in enterprises (archives)
  - Stored off-site - expensive, physical wear and tear
- AWS Storage Tape Gateway - Avoid physical tape backups
- No change needed for tape backup infrastructure
- Backup data to virtual tapes (actually, Amazon S3 & Glacier)
- Benefit from S3 features
  - encryption, high durability, low-cost, and cross-region replication
- Use S3 lifecycle management
  - move data to S3 Glacier and S3 Glacier Deep Archive