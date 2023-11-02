
# Schema Conversion Tool
- For database engines,we require a schema and code transformation before the data migration starts
- That makes heterogeneous migrations a two-step process
   - First use the AWS Schema Conversion Tool to convert the source schema and code to match that of the target database
   - Then use the AWS Database Migration Service to migrate data from the source database to the target database
  