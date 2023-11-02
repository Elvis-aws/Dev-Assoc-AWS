
# Default Termination Policies
1. Which AZ has the most instances:
   - It then selects and terminates an instance from the AZ that has the most instances
2. Which instances to terminate if allocation strategy is set between spot and on-demand instances
   - This applies if you are using lunch template where you have a mixture of spot and on-demand instances
3. If any of the instances uses the old launch configuration
   - Terminates the instance that uses the oldest launch configuration
4. If any of the instances uses the old launch template
   - Terminates the instance that uses the oldest launch template
5. Which instances are closest to the next billing hour