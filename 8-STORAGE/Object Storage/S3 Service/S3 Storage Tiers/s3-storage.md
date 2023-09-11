# Storage Classes
#################
- Transition actions
- Expiration actions
- Use Storage Lens/Storage Class Analysis to analyse your storage access
- You can enable and disable a life-cycle rule
- There is a transition cost associated with transiting
- You can use Storage Lens to view incomplete multipart uploads and use life-Cycle to expire them and save storage
- You can as well delete expired delete marker (One with no data associated with). Use Storage Lens to identify them
  and use Life-Cycle to delete them.


# Filtering
#################
- Filter with prefix
- Filter with size
- Filter with tags


##############################
# Frequent Tier
##############################
- S3 STANDARD
    - All objects created are stored in this tier
    - Milliseconds access
- S3 Standard IA
    - Milliseconds access
    - Minimum transition is 30 days
##############################
# Intelligent
##############################
- S3 Intelligent Tier
    - Automatic storage savings based on ur access pattern
    - It sends to infrequent and archive access tiers to give u savings
    - It can be used in transitioning data in data-lake, when u do not know how hot or cold ur data is.
    - It can be used for data in data-warehouses as well
    - No minimum storage duration
##############################
# Specialized Workload Tier
##############################
- S3 One Zone-IA
    - Easy re-creatable data
    - Storing different copies of data in different regions
    - Minimum transition is 30 days
- S3 Outposts
    - Delivers object storage to your on-premises AWS Outposts environment to meet local data processing
    - Using the S3 APIs and features, S3 on Outposts makes it easy to store, and control access to the data on your 
      Outpost
##############################
# Archive Tier
##############################
- S3 Glacier Instant Retrival
    - Objects access rarely may be 2x a year 
    - Retrieval in milliseconds
    - Minimum transition is 90 days
- S3 Glacier Flexible Retrival
    - Expedited (1 – 5 minutes)
    - Standard (3 – 5 hours)
    - Bulk retrievals (5–12 hours)
    - Minimum transition is 90 days
- S3 Glacier Deep Archive
    - Hours access
    - Minimum transition is 180 days
    - Standard retrieval (upto 12 hours)
    - Bulk retrieval (upto 48 hours)

