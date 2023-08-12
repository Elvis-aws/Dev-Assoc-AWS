
# Spot Instance
- A Spot Instance is an unused EC2 instance that is available for less than the On-Demand price
- Because Spot Instances enable you to request unused EC2 instances at steep discounts, you can lower your Amazon EC2 
  costs significantly
- The hourly price for a Spot Instance is called a Spot price
- The Spot price of each instance type in each Availability Zone is set by Amazon EC2 and adjusted gradually based on 
  the long-term supply of and demand for Spot Instances
# Persistent
- A Spot Instance request is either one-time or persistent
- If the spot request is persistent, the request is opened again after your Spot Instance is interrupted
- If the request is persistent and you stop your Spot Instance, the request only opens after you start your Spot Instance
# Spot blocks are designed not to be interrupted
- Spot Instances with a defined duration (also known as Spot blocks) are designed not to be interrupted and will run 
  continuously for the duration you select
- You can use a duration of 1, 2, 3, 4, 5, or 6 hours
- In rare situations, Spot blocks may be interrupted due to Amazon EC2 capacity needs
# When you cancel an active spot request, it does not terminate the associated instance
- If your Spot Instance request is active and has an associated running Spot Instance, or your Spot Instance request is 
  disabled and has an associated stopped Spot Instance, canceling the request does not terminate the instance; you must 
  terminate the running Spot Instance manually
- Moreover, to cancel a persistent Spot request and terminate its Spot Instances, you must cancel the Spot request first 
  and then terminate the Spot Instances

# Spot Concepts
1. Spot pool – Pool of EC2 instances with the same instance type, availability zone, operating system, and network platform 
2. Spot price – Current market price of a spot instance per hour as set by EC2 based on the last fulfilled bid
3. Spot bid – maximum bid price the bidder is willing to pay for the spot instance
4. Spot fleet – set of instances launched based on the criteria of the bidder
# A Spot Instance request is either
1. One-time - A one-time request remains active until EC2 launches the Spot Instance, the request expires, or you cancel 
   the request 
2. Persistent - EC2 automatically resubmits a persistent Spot request after the Spot Instance associated with the request 
   is terminated. A persistent Spot Instance request remains active until it expires or you cancel it, even if the request 
   is fulfilled. Cancelling spot instance requests does not terminate the instances. Be sure to delete the spot request 
   before you delete the instances, else they would be launched again