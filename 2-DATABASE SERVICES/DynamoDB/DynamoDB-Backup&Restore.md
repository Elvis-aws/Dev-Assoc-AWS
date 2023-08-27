
# DynamoDB Backup
- On-demand back-up:
    - Creates a full back-up or snapshot of your table
    - Long term retention
    - Regulatory compliance
- Continues backup:
    - Continues incremental back-ups
    - Restore to any second in the last 35 days
    - Exports data to S3 without affecting performance
    - You can run Athena queries on this S3 data without affecting performance
- Restore to another AWS Region
- Restore is possible without secondary indexes
- You can select encryption type during restore