
# EC2 Tenancy
- Tenancy defines how EC2 instances are distributed across physical hardware and affects pricing
  - Shared (default) 
    - You have no control of the instance location on the host as it changes address after reboot
    - You share Hypervisor with other customers
    - You share Operating System with other customers
    - You share Physical Hardware with other customers
        - CPU, RAM, Instance Store
  - Dedicated Instance (dedicated)
    - Your instance runs on single-tenant hardware
    - Provide customers with instances on dedicated hardware e.g RAM, Instance Store
    - More control over infrastructure
    - Machine address stays the same after boot
  - Dedicated Host (host)
    - Your instance runs on a physical server with EC2 instance capacity fully dedicated to your use
    - An isolated server with configurations that you can control