
# S3 Byte Range
- Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data 
  availability, security, and performance 
- Using the Range HTTP header in a GET Object request, you can fetch a byte-range from an object, transferring only the 
  specified portion
- You can use concurrent connections to Amazon S3 to fetch different byte ranges from within the same object
- This helps you achieve higher aggregate throughput versus a single whole-object request
- Fetching smaller ranges of a large object also allows your application to improve retry times when requests are 
  interrupted 
- A byte-range request is a perfect way to get the beginning of a file and ensuring we remain efficient during our scan 
  of our S3 bucket