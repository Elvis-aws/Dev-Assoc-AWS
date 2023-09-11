
# EC2 Spot Block and Spot Fleet
- Spot Block
  - Allow you to request Spot instances for a specific duration (1 or 2 or .. or 6 hours)
  - Recommended for jobs that take finite time to complete
- Spot Fleet
  - Using Spot Fleet, you can request spot instances across a range of instance types
  - Advantage : The more instance types that you specify, the better your chances of having your target capacity fulfilled
# EC2 Spot Instances - Remember
- Spot instances can be terminated, stopped, or hibernated when interrupted
  - Default - terminated 
  - Use maintain option while creating spot request for stop and hibernate options 
  - Hibernating a Spot instance allows you to save state of EC2 instances and quickly start up
- To completely close a spot request:
  - Step 1. Cancel Spot Request 
  - Step 2. Terminate all Spot Instances
- (Remember) Canceling a spot request might not terminate active spot instances