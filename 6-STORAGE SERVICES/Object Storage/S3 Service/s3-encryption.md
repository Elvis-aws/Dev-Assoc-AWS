
# S3 Encryption
- AWS S3 Encryption supports both data at rest and data in transit encryption
- Data in-transit
    - S3 allows protection of data in transit by enabling SSL or using client-side encryption
- Data at Rest
    - Server-Side Encryption
        - S3 encrypts the object before saving it on disks 
        - Server-side encryption encrypts only the object data
        - Any object metadata is not encrypted
        - Encrypted and unencrypted objects and is handled transparently by S3
    - S3-Managed Keys – SSE-S3
        - Encryption keys are handled and managed by AWS
        - SSE-S3 encrypts the data key with a master key that is regularly rotated
        - Uses 256-bit Advanced Encryption Standard (AES-256)
        - Request must set header x-amz-server-side-encryption to AES-256
        - For enforcing server-side encryption for all of the objects, use a bucket policy that denies permissions to 
          upload an object unless the request includes x-amz-server-side-encryption header
    - AWS KMS-Managed Keys – SSE-KMS
        - KMS uses customer master keys (CMKs) to encrypt the S3 objects
        - The master key is never made available
        - Allows keys to be rotated regularly
        - Allows audit of keys used to prove they are being used correctly, by inspecting logs in AWS CloudTrail
        - Security controls in AWS KMS can help meet encryption-related compliance requirements
        - SSE-KMS provides the option to create and manage encryption keys yourself, or use a default customer master key
        - S3 only supports symmetric keys and not asymmetric keys
        - Must set header x-amz-server-side-encryption to aws:kms
    - Customer-Provided Keys – SSE-C
        - Encryption keys can be managed and provided by the Customer and S3 manages the encryption
        - When you upload an object, the encryption key is provided as a part of the request and S3 uses that encryption 
          key to apply AES-256 encryption
        - SSE-C requests must be done through HTTPS and S3 will reject any requests made over HTTP when using SSE-C
    - Client-Side Encryption
        - Data is encrypted at the client-side and uploaded to S3
        - The encryption process, the encryption keys, and related tools are managed by the user
        - Client-side master keys and your unencrypted data are never sent to AWS
        - If the master key is lost the data cannot be decrypted