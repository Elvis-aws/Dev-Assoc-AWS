
# AWS DynamoDB
- It is a hosted NoSQL database
- Scales infinitely
- JOINs and advanced SQL operations can slow down your queries
- DynamoDB is accessible via an HTTP API
- Performs authentication & authorization via IAM roles
- Amazon DynamoDB lets you specify the desired consistency
    - Eventually consistent: Does not always reflect the results of a recently completed write
    - Strongly consistent: Returns a result that reflects all writes that received a successful response 
                           It takes more resources to process a strongly consistent read 