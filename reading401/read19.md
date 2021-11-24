# Readings: AWS: Events


## Review, Research, and Discussion
1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server
    - Deploying Express Gateway is going to be very different from Amazon API Gateway because it is not a hosted solution. You have numerous options for hosting Express Gateway, including running Node.js on Amazon EC2 or using Docker with Amazon ECS. Unlike Amazon API Gateway, Express Gateway can store users in Redis, independent of any centralized auth setup like AWS IAM. Express Gateway can also run without a backend data store, but it should be noted that without a backend data store your users will be lost if your Express Gateway server restarts.
2. List the AWS Database offerings and talk about the pros and cons of each
    - **Pros**
        - Supports many types of databases like MySQL, PostgreSQL, Aurora, etc.
        - RDS console makes it very easy to maintain all the different instances of relational database services.
        - Provides performance insights for all the database instances.
    - **Cons**
        - Cost is very high as compared to other cloud service providers.
        - Snapshots are also very expensive to maintain.
3. What’s the difference between a FIFO and a standard queue?
    - Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.
4. How can the server be assured a message was properly received?
    - The client sends a request, and the server returns a response. This exchange of messages is an example of inter-process communication. To communicate, the computers must have a common language, and they must follow rules so that both the client and the server know what to expect.

 ## DOCUMENTATION:
Serverless API
:  Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider

Triggers
:   anything that might cause a person to recall a traumatic experience they've had. 

Dynamo vs Mongo
:  Both these databases support multi-document transactions, but with key differences: MongoDB supports read and writes to the same documents and fields in a single database transaction. DynamoDB lacks support for multiple operations within a single transaction

Dynamoose vs Mongoose   
:  Dynamoose is obviously inspired by mongoose and is a good choice if you have a well-defined schema and/or want to be abstracted away from the DynamoDB details