
# S3 Select
- With Amazon S3 Select, you can use structured query language (SQL) statements to filter the contents of an Amazon S3 
  object and retrieve only the subset of data that you need 
- Amazon S3 Select works on objects stored in CSV, JSON, or Apache Parquet format
# Requirements and limits
- You must have s3:GetObject permission for the object you are querying
- If the object you are querying is encrypted with server-side encryption with customer-provided keys (SSE-C), you must 
  use https, and you must provide the encryption key in the request 
- The maximum length of a SQL expression is 256 KB
- The maximum length of a record in the input or result is 1 MB
- Amazon S3 Select can only emit nested data by using the JSON output format
- You cannot query objects in the S3 Glacier Flexible Retrieval, S3 Glacier Deep Archive, or Reduced Redundancy Storage 
  (RRS) storage classes. You also cannot query the objects in the S3 Intelligent-Tiering Archive Access tier or the S3 
  Intelligent-Tiering Deep Archive Access tier