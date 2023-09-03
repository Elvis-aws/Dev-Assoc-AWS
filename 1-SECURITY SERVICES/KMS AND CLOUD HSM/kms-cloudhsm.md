
# KMS and Cloud HSM
- How do you generate, store, use and replace your keys?
- AWS provides two important services - KMS and Cloud HSM
  - Manage your keys 
  - Perform encryption and decryption
# AWS KMS
- Create and manage cryptographic keys (symmetric and asymmetric)
- Control their use in your applications and AWS Services
- Define key usage permissions (including cross account access)
- Track key usage in AWS CloudTrail (regulations & compliance)
- Integrates with almost all AWS services that need data encryption
- Automatically rotate master keys once a year
  - No need to re-encrypt previously encrypted data (versions of master key are maintained)
- Schedule key deletion to verify if the key is used
  - Mandatory minimum wait period of 7 days (max-30 days)
- AWS KMS supports multi-region keys
# Server Side Encryption with KMS
- Create Customer Master Key. Map to AWS service (S3)
# Steps
- Data sent to S3 
- S3 receives data keys from KMS 
- S3 encrypts data 
- Stores encrypted data & data key
# Remember
- CMK never leaves KMS
- Encryption of data key - KMS using CMK
- Encryption of data - AWS Service - Amazon S3 using data key
# Envelope Encryption
- The process KMS uses for encryption is called Envelope Encryption
  - Data is encrypted using data key 
  - Data key is encrypted using Master key 
  - Master key never leaves KMS
- KMS encrypts small pieces of data (usually data keys) less than 4 KB
# Decryption of data using KMS
- AWS service (Amazon S3) sends encrypted data key to KMS
- KMS uses Customer Master Key (CMK) to decrypt and return plain-text data key
- AWS service (Amazon S3) uses the plain-text data key to perform decryption
- (TIP) Remove plain-text data key from memory asap
- (TIP) AWS service needs IAM permissions to use the CMK
# Remember:
- (Optional) You can associate a key/value map called encryption context with any cryptographic operation
- (TIP) If encryption context is different, decryption will NOT succeed

# AWS CloudHSM
- Managed (highly available & auto scaling) dedicated single-tenant Hardware Security Module(HSM) for regulatory compliance
- (Remember) AWS KMS is a multi-tenant service
- FIPS 140-2 Level 3 compliant
- AWS CANNOT access your encryption master keys in CloudHSM
- In KMS, AWS can access your master keys
- Be ultra safe with your keys when you are using CloudHSM
- (Recommendation) Use two or more HSMs in separate AZs in a production cluster
# Use cases
- (Web servers) Offload SSL processing
- Certificate Authority
- Digital Rights Management
- TDE for Oracle databases
