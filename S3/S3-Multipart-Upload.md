
# Multi-Part-Upload
- Multipart upload allows you to upload a single object as a set of parts. 
- Each part is a contiguous portion of the object's data. 
- You can upload these object parts independently and in any order. 
- If transmission of any part fails, you can retransmit that part without affecting other parts. 
- After all parts of your object are uploaded, Amazon S3 assembles these parts and creates the object. 
- In general, when your object size reaches 100 MB, you should consider using multipart uploads instead of uploading 
  the object in a single operation

# CLI
- file name = myfile.mp4
- bucket name = mybucket
- First split ur large file ( split -b 40m myfile.mp4)
    - xaa
    - xab
    - xac
- Create multipart UploadId to upload ur parts
    - aws s3api create-multipart-upload --bucket mybucket --key myfile.mp4
- UploadId = h1b2n3m4n5
- Start uploading ur split files
    - aws s3api upload-part --bucket mybucket --key myfile.mp4 --part-number 1 --body xaa --upload-id h1b2n3m4n5
    - aws s3api upload-part --bucket mybucket --key myfile.mp4 --part-number 2 --body xab --upload-id h1b2n3m4n5
    - aws s3api upload-part --bucket mybucket --key myfile.mp4 --part-number 3 --body xac --upload-id h1b2n3m4n5
- Copy the ETag value as a reference for later steps
- After you upload all the file parts, run the following command to confirm that the list is complete
    - aws s3api list-parts --bucket mybucket --key myfile.mp4 --upload-id h1b2n3m4n5
      - Compile the ETag values for each file part that you uploaded into a JSON-formatted file.
      - File name = fileparts.json
      {
          "Parts": [{
              "ETag": "example8be9a0268ebfb8b115d4c1fd3",
              "PartNumber":1
          },

          {
              "ETag": "example8be9a026763hegtt63gghdy33",
              "PartNumber":2
          },

          {
              "ETag": "example246e31ab807da6f62802c1ae8",
              "PartNumber":3
          }]
      }
- Complete the multipart upload
    - aws s3api complete-multipart-upload --multipart-upload file://fileparts.json --bucket mybucket --key myfile.mp4 --upload-id h1b2n3m4n5
- If the upload fails, remove incomplete parts of the upload, and then re-upload the parts
    - aws s3api list-multipart-uploads --bucket mybucket
    - aws s3api abort-multipart-upload --bucket mybucket --key myfile.mp4 --upload-id h1b2n3m4n5
- Use AbortIncompleteMultipartUpload Lifecycle configuration action in the bucket life cycle to determine how long 
  unsuccessful multiparts should stay in the bucket

# Python
- Create Multi-part upload creates an id
- This id is just a reference
- You won't see this file in S3 until the process is complete
- You can upload parts of the file into a new file
- We can retry sections if they fail bc it just overwrites what was there
- At the end of the last upload, only then can u see this file in S3