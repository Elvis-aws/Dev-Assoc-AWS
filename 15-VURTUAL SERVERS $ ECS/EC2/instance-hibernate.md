
# EC2 Instance Hibernate
- Hibernation saves the contents from the instance memory (RAM) to your Amazon Elastic Block Store (Amazon EBS) root volume
- Amazon EC2 persists the instance's EBS root volume and any attached EBS data volumes
- When you start your instance: The EBS root volume is restored to its previous state
# Benefit of Hibernating over Stopping
1. The memory state is preserved
2. Since the memory state is perserved and loaded again when the instance start, this reduce the boot time of the instance 
3. The long running process can continue without interuption 
4. A great benefit if you have some services that take a great amount of time to fully initialized