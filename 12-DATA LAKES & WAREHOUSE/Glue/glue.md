
# AWS Glue
- AWS Glue is a Fully managed extract, transform, and load (ETL) service in AWS
# Here are some of the important characteristics to remember:
- Simplify data preparation (capturing metadata) for analytics:
  - Connect AWS Glue to your data on AWS (Aurora, RDS, Redshift, S3 etc)
  - AWS Glue creates a AWS Glue Data Catalog with metadata abstracted from your data
  - Your data is ready for searching and querying
- Run your ETL jobs using Apache Spark
- Metadata from AWS Glue Data Catalog can be used from:
  - Amazon Athena
  - Amazon EMR
  - Amazon Redshift Spectrum