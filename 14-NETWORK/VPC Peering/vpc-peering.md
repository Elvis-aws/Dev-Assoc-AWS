
# VPC peering
- VPC Peering helps you to connect VPCs belonging to same or different AWS accounts irrespective of the region of the VPCs
- This allows private communication between the connected VPCs
- Peering uses a request/accept protocol:
  - Owner of requesting VPC sends a request 
  - Owner of the peer VPC has one week to accept
- Couple of important things to remember about VPC Peering:
  - Peering is not transitive 
  - Peer VPCs cannot have overlapping address ranges (CIDR or subnets)
  - Peering is not possible with on-premise servers