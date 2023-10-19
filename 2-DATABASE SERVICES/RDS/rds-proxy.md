
# AWS RDS Proxy
- Amazon RDS Proxy is a fully managed, highly available database proxy for Amazon Relational Database Service (RDS) that 
  makes applications more scalable, more resilient to database failures, and more secure
- Many applications, including those built on modern serverless architectures, can have a large number of open connections 
  to the database server and may open and close database connections at a high rate, exhausting database memory and compute 
  resources
- Amazon RDS Proxy allows applications to pool and share connections established with the database, improving database 
  efficiency and application scalability
- With RDS Proxy, failover times for Aurora and RDS databases are reduced by up to 66%, and database credentials, 
  authentication, and access can be managed through integration with AWS Secrets Manager and AWS Identity and Access 
  Management (IAM)
- Amazon RDS Proxy can be enabled for most applications with no code changes, and you don’t need to provision or manage 
  any additional infrastructure
- Pricing is simple and predictable: you pay per vCPU of the database instance for which the proxy is enabled
- Amazon RDS Proxy is now generally available for Aurora MySQL, Aurora PostgreSQL, RDS MySQL, and RDS PostgreSQL

