
# Glacier Vault Storage
- Glacier Vault is an archive storage solution independent from AWS S3
- It uses storage containers named vaults (opposed to S3 buckets) and its own set of APIs for data uploading and 
  retrieving
- As the storage price is cheaper compared to S3, data retrieval is more expensive and time-consuming
- However, both of these properties can be influenced by applying a retrieval policy specific to the use case
  - standard (aimed at cost-effective retrieval of big datasets) 3-5 hrs
  - Bulk (aimed at cost-effective retrieval of big datasets) 5-12 hrs
  - Expedited policy (aimed at faster retrieval of data) 1-5 mins
- Once uploaded, the dataset stored in the Glacier vault can be listed by requesting the metadata with an API request
- Typically, it takes about 4 hours to retrieve metadata which in turn clears the way for full or partial retrieval of 
  the dataset 
- The vault where the data is stored can also be applied with a vault lock which prevents locked data deletion for a 
  specified period 
- Despite Glacier Vault storage is no longer actively developed by Amazon, it is still functional