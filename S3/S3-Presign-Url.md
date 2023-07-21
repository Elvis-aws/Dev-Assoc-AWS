
# Pre-sign-Url
- We have a private bucket
- Our clients can interact with this bucket using S3-Presign-Url
- Create bucket
- Go to permissions and add cors (headers, methods, origin)
- Create an api with S3 client
- Add signatureVersion: 'v4' to the client
- Define an object s3-params =  {key, Expires, ContentType}
- create the presignedUrl = await s3.getSignedUrl('putObject',s3-params)
- Return the pre-signed url
- The user can use this url to upload files, in the duration set and only the specified key or filetype