
# Amazon S3 access control lists
- ACL is disabled by default
- ACL enables you to manage access to buckets and objects when enabled
- Each bucket and object has an ACL attached to it as a subresource
- It defines which AWS accounts or groups are granted access and the type of access
- When a request is received against a resource, Amazon S3 checks the corresponding ACL to verify that the requester 
  has the necessary access permissions 
# ACL Object Ownership
- It is an Amazon S3 bucket-level setting that you can use to both control ownership of the objects that are uploaded to 
  your bucket and to disable or enable ACLs
- By default, it is set to the bucket owner enforced setting, and all ACLs are disabled
- When ACLs are disabled, the bucket owner owns all the objects in the bucket and manages access to them exclusively by 
  using access-management policies 
- A majority of modern use cases in Amazon S3 no longer require the use of ACLs
- We recommend that you keep ACLs disabled, except in unusual circumstances where you need to control access for each 
  object individually
- With ACLs disabled, you can use policies to control access to all objects in your bucket, regardless of who uploaded 
  the objects to your bucket
- If your bucket uses the bucket owner enforced setting for S3 Object Ownership, you must use policies to grant access 
  to your bucket and the objects in it
- With the bucket owner enforced setting enabled, requests to set access control lists (ACLs) or update ACLs fail and 
  return the AccessControlListNotSupported error code. Requests to read ACLs are still supported