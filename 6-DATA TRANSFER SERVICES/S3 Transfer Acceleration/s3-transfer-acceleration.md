
# S3-Performance
- Most basic option when you are transferring less data (upto a few terabytes) into S3
- It uses the globally distributed CloudFront edge network
- It helps reduce latency by speeding up uploads and downloads
- It can be enabled/suspend on a bucket on properties tab
- Transfer acceleration endpoint is enabled and displayed
- You can compare direct S3 upload vs Transfer acceleration speed
- Use code to upload and download our image
- Set transfer acceleration to true in the S3 Client
- S3 uploads the file from the destination bucket and stores in an Edge location
- Using the private AWS network
- This is an s3 service and can only transfer objects