
# AWS Directory Service
- Provide AWS access to on-premise users without IAM users
- Managed service deployed across multiple AZs
- Option 1 : AWS Directory Service for Microsoft AD
  - More than 5000 Users
  - Trust relationship needed between AWS and on-premise directory
- Option 2 : Simple AD
  - Less than 5000 users
  - Powered by Samba4 and compatible with Microsoft AD
  - Does not support trust relationships with other AD domains
- Option 3 : AD Connector
  - Use your existing on-premise directory with AWS cloud services
  - Your users use existing credentials to access AWS resources