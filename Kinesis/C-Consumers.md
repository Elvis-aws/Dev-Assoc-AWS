
# Kinesis consumers
- A consumer is an application that processes all data from a Kinesis data stream
- When a consumer uses enhanced fan-out, it gets its own 2 MB/sec allotment of read throughput, allowing multiple 
  consumers to read data from the same stream in parallel, without contending for read throughput with other consumers