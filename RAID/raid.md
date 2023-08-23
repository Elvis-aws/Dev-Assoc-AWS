
# RAID 0
- Creating a RAID 0 array allows you to achieve a higher level of performance for a file system than you can provision 
  on a single Amazon EBS volume
- Use RAID 0 when I/O performance is of the utmost importance
- With RAID 0, I/O is distributed across the volumes in a stripe
# RAID 1
- RAID 1, also known as mirroring, involves creating two EBS volumes and duplicating data between them
- Data is written to both volumes simultaneously, providing redundancy in case of a failure of one volume
- RAID 1 can improve read performance but may result in a slight decrease in write performance