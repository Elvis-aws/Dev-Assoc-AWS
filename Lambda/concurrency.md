
# Concurrency
- In Lambda, concurrency is the number of in-flight requests your function is handling at the same time
- There are two types of concurrency controls available
-  Each region in your AWS account has a Lambda concurrency limit
- The limit applies to all functions in the same region and is set to 1000 by default
- You need to contact AWS support to raise the account limit if function invocation hits this limit
# Reserved concurrency 
- Reserved concurrency is the maximum number of concurrent instances you want to allocate to your function
- When a function has reserved concurrency, no other function can use that concurrency
- There is no charge for configuring reserved concurrency for a function
# Provisioned concurrency
- Provisioned concurrency is the number of pre-initialized execution environments you want to allocate to your function
- These execution environments are prepared to respond immediately to incoming function requests
- Configuring provisioned concurrency incurs charges to your AWS account

