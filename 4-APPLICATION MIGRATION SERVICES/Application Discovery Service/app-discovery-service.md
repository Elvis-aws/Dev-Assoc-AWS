
# AWS Application Discovery Service 
- It collects and presents data to enable customers to understand the configuration, usage, and behavior of servers
- Server data is retained in the Application Discovery Service where it can help organize AWS migration planning
- Collected data can be exported for analysis in Excel or other cloud migration analysis tools
- It helps enterprises obtain a snapshot of the current state of their data center servers
- It helps create a cost optimized migration plan based on your unique business requirements
# Agentless discovery
- Suited for VMware
- Deploying the Application Discovery Service Agentless Collector through your VMware vCenter
- After Agentless Collector is configured, it identifies virtual machines (VMs) and hosts associated with vCenter
- It collects the following static configuration data: 
    - Server hostnames
    - IP addresses
    - MAC addresses
    - disk resource allocations
    - database engine versions
    - database schemas
# Agent-based discovery 
- Suited for non VMware machines having Windows, Linux, Ubuntu, CentOS operating systems
- Deploying the AWS Application Discovery Agent on each of your VMs and physical servers
- The agent installer is available for Windows and Linux operating systems
- It collects static configuration data:
    - detailed time-series 
    - system-performance information
    - inbound and outbound network connections
    - processes that are running