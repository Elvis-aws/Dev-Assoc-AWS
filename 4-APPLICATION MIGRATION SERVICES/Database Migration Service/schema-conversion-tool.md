
# Schema Conversion Tool
- If the source and target databases engines are different, like in the case of Oracle to Amazon Aurora, Oracle to 
  PostgreSQL, we thus require a schema and code transformation before the data migration starts
- That makes heterogeneous migrations a two-step process. First use the AWS Schema Conversion Tool to convert the source 
  schema and code to match that of the target database, and then use the AWS Database Migration Service to migrate data 
  from the source database to the target database
  