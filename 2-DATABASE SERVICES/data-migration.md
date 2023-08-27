
# Amazon Redshift database as a target
- You can migrate data to Amazon Redshift databases using AWS Database Migration Service
- Amazon Redshift is a fully managed, petabyte-scale data warehouse service in the cloud
- With an Amazon Redshift database as a target, you can migrate data from all of the other supported source databases
- The Amazon Redshift cluster must be in the same AWS account and the same AWS Region as the replication instance
- During a database migration to Amazon Redshift, AWS DMS first moves data to an Amazon S3 bucket
- When the files reside in an Amazon S3 bucket, AWS DMS then transfers them to the proper tables in the Amazon Redshift 
  data warehouse
- AWS DMS creates the S3 bucket in the same AWS Region as the Amazon Redshift database
- The AWS DMS replication instance must be located in that same region