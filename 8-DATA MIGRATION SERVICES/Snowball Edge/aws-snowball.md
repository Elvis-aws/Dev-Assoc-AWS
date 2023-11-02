
# AWS Snowball
- Transfer dozens of terabytes to petabytes of data from on-premises to AWS
- 100TB (80 TB usable) per appliance
- Involves physical shipping
- Simple Process
  - Request for Snowball
  - Copy data
  - Ship it back
- Data is automatically encrypted with KMS (AES-256)
- Choose between
  - Storage optimized (24 vCPUs, 32 GiB RAM)
  - Compute optimized(52 vCPUs, 208 GiB RAM)
  - Compute optimized with GPU
- Choose Snowball if direct transfer takes over a week
  - 5TB can be transferred on 100Mbps line in a week at 80% utilization