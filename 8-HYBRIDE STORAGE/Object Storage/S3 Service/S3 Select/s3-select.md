
# S3 Select
- 3 Select is a new Amazon S3 capability designed to pull out only the data you need from an object, which can dramatically 
  improve the performance and reduce the cost of applications that need to access data in S3
# Exam Alert:
- Please note that with Amazon S3 Select, you can scan a subset of an object by specifying a range of bytes to query using 
  the ScanRange parameter
- This capability lets you parallelize scanning the whole object by splitting the work into separate Amazon S3 Select 
  requests for a series of non-overlapping scan ranges
- Use the Amazon S3 Select ScanRange parameter and Start at (Byte) and End at (Byte)