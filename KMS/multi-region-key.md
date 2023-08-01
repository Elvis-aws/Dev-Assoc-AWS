
# Multi-Region Key
- AWS KMS supports multi-region keys, which are AWS KMS keys in different AWS regions that can be used interchangeably
  as though you had the same key in multiple regions
- Each set of related multi-region keys has the same key material and key ID, so you can encrypt data in one AWS region 
  and decrypt it in a different AWS region without re-encrypting or making a cross-region call to AWS KMS
- You can use multi-region AWS KMS keys in Amazon S3
- However, Amazon S3 currently treats multi-region keys as though they were single-region keys, and does not use the 
  multi-region features of the key
# Data Transfer to another bucket
1. Create a new bucket in the destination region
2. Enable replication
3. Enable SSE-KMS encryption on the new bucket
4. Use the multi-region key (encrypted and decrypted data)
5. copy any existing data