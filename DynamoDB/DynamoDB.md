
# AWS DynamoDB
- It is a hosted NoSQL database
- Scales infinitely
- As your amount of data scales, JOINs and advanced SQL operations can slow down your queries. With DynamoDB, 
  your queries have predictable latency up to any size, including over 100 TBs
- AWS Lambda provides auto-scaling, stateless, ephemeral compute in response to event triggers. DynamoDB is accessible 
  via an HTTP API and performs authentication & authorization via IAM roles, making it a perfect fit for building 
  Serverless applications
- Amazon DynamoDB lets you specify the desired consistency characteristics for each read request within an application
    - Eventually consistent: An eventually consistent read might not always reflect the results of a recently completed 
      write
    - Strongly consistent: returns a result that reflects all writes that received a successful response prior to the 
      read. It takes more resources to process a strongly consistent read than an eventually consistent read