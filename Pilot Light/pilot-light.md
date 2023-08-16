
# Pilot Light
- The term pilot light is often used to describe a DR scenario in which a minimal version of an environment is always 
  running in the cloud
- The idea of the pilot light is an analogy that comes from the gas heater
- In a gas heater, a small flame that’s always on can quickly ignite the entire furnace to heat up a house
- This scenario is similar to a backup-and-restore scenario. For example, with AWS you can maintain a pilot light by 
  configuring and running the most critical core elements of your system in AWS
- A small part of the backup infrastructure is always running simultaneously syncing mutable data (such as databases or 
  documents) so that there is no loss of critical data
- When the time comes for recovery, you can rapidly provision a full-scale production environment around the critical core
- For Pilot light, RPO is in minutes