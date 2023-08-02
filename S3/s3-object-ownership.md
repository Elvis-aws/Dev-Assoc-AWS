
# Object Ownership
- By default, an S3 object is owned by the AWS account that uploaded it
- This is true even when the bucket is owned by another account
- When ACLs are disabled, the bucket owner owns all the objects in the bucket and manages access to data exclusively 
  using access management policies
- A majority of modern use cases in Amazon S3 no longer require the use of ACLs, and we recommend that you keep ACLs 
  disabled. With ACLs disabled, you can use policies to more easily control access to every object in your bucket, 
  regardless of who uploaded the objects in your bucket