
# EC2 Instance Hibernate
- Hibernation saves the contents from the instance memory (RAM) to your Amazon Elastic Block Store (Amazon EBS) root volume
- Amazon EC2 persists the instance's EBS root volume and any attached EBS data volumes
- When you start your instance: The EBS root volume is restored to its previous state
# Benefit of Hibernating over Stopping
1. The memory state is preserved
2. Since the memory state is preserved and loaded again when the instance start, this reduces the boot time of the instance 
3. The long-running process can continue without interruption 
4. A great benefit if you have some services that take a great amount of time to fully initialized 
5. Memory intensive applications or those that require a long time to boot-strap 
6. Hibernate pre-warms the instance and after resuming it, it quickly brings all application processes in running state