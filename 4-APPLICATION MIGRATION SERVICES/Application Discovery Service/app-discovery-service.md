
# AWS Application Discovery Service 
- It collects and presents data to enable enterprise customers to understand the configuration, usage, and behavior of 
  servers in their IT environments
- Server data is retained in the Application Discovery Service where it can be tagged and grouped into applications to 
  help organize AWS migration planning
- Collected data can be exported for analysis in Excel or other cloud migration analysis tools
- It helps enterprises obtain a snapshot of the current state of their data center servers by collecting server 
  specification information, hardware configuration, performance data, and details of running processes and network 
  connections
- Once the data is collected, you can use it to perform a Total Cost of Ownership (TCO) analysis and then create a cost 
  optimized migration plan based on your unique business requirements
- Ways of performing discovery and collecting data about your on-premises servers are as below
# Agentless discovery
- Suited for VMware
- Can be performed by deploying the Application Discovery Service Agentless Collector (Agentless Collector) (OVA file) 
  through your VMware vCenter
- After Agentless Collector is configured, it identifies virtual machines (VMs) and hosts associated with vCenter
- Agentless Collector collects the following static configuration data: Server hostnames, IP addresses, MAC addresses, 
  disk resource allocations, database engine versions, and database schemas
- Additionally, it collects the utilization data for each VM and database providing the average and peak utilization for 
  metrics such as CPU, RAM, and Disk I/O
# Agent-based discovery 
- Suited for non VMware machines having Windows, Linux, Ubuntu, CentOS operating systems
- Can be performed by deploying the AWS Application Discovery Agent on each of your VMs and physical servers
- The agent installer is available for Windows and Linux operating systems
- It collects static configuration data, detailed time-series system-performance information, inbound and outbound 
  network connections, and processes that are running
- Application Discovery Service integrates with application discovery solutions from AWS Partner Network (APN) partners
- These third-party solutions can help you import details about your on-premises environment directly into Migration Hub, 
  without using any agentless collector or discovery agent
- Third-party application discovery tools can query AWS Application Discovery Service, and they can write to the 
  Application Discovery Service database using the public API
- In this way, you can import data into Migration Hub and view it, so that you can associate applications with servers 
  and track migrations