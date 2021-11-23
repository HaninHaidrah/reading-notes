# Readings: AWS: API, Dynamo and Lambda


## Review, Research, and Discussion
1. What are serverless functions?
    - A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier 

2. If you were to create a system that emulated Lambda functions, how would you do it?
    - To create a Lambda function with the console: 

        > Open the Functions page of the Lambda console.

        > Choose Create function.

        > Under Basic information, do the following:

        > For Function name, enter my-function.

        > For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.

       > Choose Create function.

3. Describe how a CDN works
    - A CDN is a network of servers that distributes content from an “origin” server throughout the world by caching content close to where each end user is accessing the internet via a web-enabled device.

## DOCUMENTATION:
Serverless Functions
:  is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier 

Cloud Storage
:  refers to software and services that run on the Internet, instead of locally on your computer. Most cloud services can be accessed through a Web browser like Firefox or Google Chrome, and some companies offer dedicated mobile apps.
![IMG](http://lsinet.co.uk/wp-content/uploads/2019/09/cloud-computing.png)

CDN
:   a network of servers that distributes content from an “origin” server throughout the world by caching content close to where each end user is accessing the internet via a web-enabled device.

![img](https://www.imperva.com/wp-content/uploads/sites/13/2020/03/diagram-12@3x.png)


## Preview
 ***Amazon API Gateway*** =>  is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

 **DynamoDB** => is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

* reliable performance even as it scales;
    - a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
    - a small, simple API allowing for simple key-value access as well as more advanced query patterns.
    - DynamoDB is a particularly good fit for the following use cases:

* When we can use :    

    - Applications with large amounts of data and strict latency requirements. As your amount of data scales, JOINs and advanced SQL operations can slow down your queries. With DynamoDB, your queries have predictable latency up to any size, including over 100 TBs!

    - Serverless applications using AWS Lambda. AWS Lambda provides auto-scaling, stateless, ephemeral compute in response to event triggers. DynamoDB is accessible via an HTTP API and performs authentication & authorization via IAM roles, making it a perfect fit for building Serverless applications.

    - Data sets with simple, known access patterns. If you're generating recommendations and serving them to users, DynamoDB's simple key-value access patterns make it a fast, reliable choice. [source](https://www.dynamodbguide.com/what-is-dynamo-db/)