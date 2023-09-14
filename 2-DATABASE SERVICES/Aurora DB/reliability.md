
# Amazon Aurora reliability
- Aurora is designed to be reliable, durable, and fault tolerant
- You can architect your Aurora DB cluster to improve availability by doing things such as adding Aurora Replicas and 
  placing them in different Availability Zones, and also Aurora includes several automatic features that make it a 
  reliable database solution
# Storage auto-repair
  - Because Aurora maintains multiple copies of your data in three Availability Zones, the chance of losing data as a 
    result of a disk failure is greatly minimized. Aurora automatically detects failures in the disk volumes that make 
    up the cluster volume. When a segment of a disk volume fails, Aurora immediately repairs the segment
# Survivable page cache
  - In Aurora, each DB instance's page cache is managed in a separate process from the database, which allows the page 
    cache to survive independently of the database. In the unlikely event of a database failure, the page cache remains 
    in memory, which keeps current data pages "warm" in the page cache when the database restarts
# Crash recovery
  - Aurora is designed to recover from a crash almost instantaneously and continue to serve your application data without 
    the binary log. Aurora performs crash recovery asynchronously on parallel threads, so that your database is open 
    and available immediately after a crash