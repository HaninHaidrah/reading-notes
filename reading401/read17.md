# Readings: AWS: S3 and Lambda
## Review, Research, and Discussion
1. Describe “The Cloud”
    - The cloud refers to software and services that run on the Internet, instead of locally on your computer. Most cloud services can be accessed through a Web browser like Firefox or Google Chrome, and some companies offer dedicated mobile apps.
2. What is a container (as it relates to computers and servers)?
    - A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.
3. What is auto-scaling?
    - AWS Auto Scaling monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. Using AWS Auto Scaling, it's easy to setup application scaling for multiple resources across multiple services in minutes.
4. What is bandwidth?
    - The maximum amount of data transmitted over an internet connection in a given amount of time. Bandwidth is often mistaken for internet speed when it's actually the volume of information that can be sent over a connection in a measured amount of time – calculated in megabits per second (Mbps).
5. How do cloud providers compute service costs?
    - When setting price, cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. 

 ## DOCUMENTATION: 
Server Instances
:  is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

Containers
:  is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

Cloud Services
:  refers to software and services that run on the Internet, instead of locally on your computer. Most cloud services can be accessed through a Web browser like Firefox or Google Chrome, and some companies offer dedicated mobile apps.
![IMG](http://lsinet.co.uk/wp-content/uploads/2019/09/cloud-computing.png)

Cloud Architecture
:  refers to the various components in terms of databases, software capabilities, applications
![IMG](https://www.redhat.com/cms/managed-files/styles/wysiwyg_full_width/s3/Screen%20Shot%202019-06-24%20at%202.27.06%20PM.png?itok=7yByods-)

AWS
:  is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis

EC2/Beanstalk vs Heroku  
:  One big difference is that Heroku's pricing takes exponential price jumps as one adds common additional features


## Preview

***Amazon Simple Storage Service (Amazon S3)***=> is an object storage service offering industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can store and protect any amount of data for virtually any use case, such as data lakes, cloud-native applications, and mobile apps. With cost-effective storage classes and easy-to-use management features, you can optimize costs, organize data, and configure fine-tuned access controls to meet specific business, organizational, and compliance requirements.
![img](https://d1.awsstatic.com/s3-pdp-redesign/product-page-diagram_Amazon-S3_HIW%402x.ee85671fe5c9ccc2ee5c5352a769d7b03d7c0f16.png)

***Lambda function*** => runs in its own container. When a function is created, Lambda packages it into a new container and then executes that container on a multi-tenant cluster of machines managed by AWS. Before the functions start running, each function’s container is allocated its necessary RAM and CPU capacity. Once the functions finish running, the RAM allocated at the beginning is multiplied by the amount of time the function spent running. The customers then get charged based on the allocated memory and the amount of run time the function took to complete.