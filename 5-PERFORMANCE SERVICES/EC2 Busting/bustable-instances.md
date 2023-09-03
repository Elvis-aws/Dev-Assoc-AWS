
# EC2 Burstable Instances (T family - T2, T3 etc)
- There are special type of EC2 instances called Burstable instances
- These instances gather CPU Credits while they are idle
- The CPU credits can be consumed at a later point in time (upto a maximum CPU Credit)
# Use case: 
- Workloads with sudden spikes - Test environments
- You can also use Unlimited Mode - Spike beyond CPU credit at additional cost:
  - For T2 instances, Unlimited Mode is disabled by default
  - For T3 instances, Unlimited Mode is enabled by default