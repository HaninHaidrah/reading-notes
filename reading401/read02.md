# Readings: Express

## Review, Research, and Discussion:
1. What’s the difference between PUT and PATCH?
    * PUT => completly updating the data (send all of the information thorugh request.body)
    * PATCH => partly updating (update some data not all )
2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
    * [POSTMAN](https://www.postman.com/)
    * [WIREMOCK](http://wiremock.org/)
    * [MOCKOON](https://mockoon.com/)
3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?
    * swagger => **HTTP Status Codes**
        *Under responses, each response definition starts with a status code, such as 200 or 404. An operation typically returns one successful status code and one or more error statuses. To define a range of response codes, you may use the following range definitions: 1XX, 2XX, 3XX, 4XX, and 5XX.*
    *  APIDoc.js => **HTTP Status Codes**
        *Status codes don’t appear in the response body. They appear in the response header, which you might not see by default.*
4. Compare and contrast SOAP and ReST
    * SOAP => 
        - Simple Object Access Protocol – is probably the better known of the two models.
        - SOAP relies heavily on XML, and together with schemas
        - Each input parameter is similarly defined and bound to a type
        -
    * REST => 
        - REpresentational State Transfer– is quickly becoming the preferred design model for public APIs
        - It  relies on a stateless communications protocol, most commonly, HTTP. REST structures data in XML, YAML, or any other format that is machine-readable, but usually JSON is most widely used.
        - There is no standard for the description format of REST services 


## Documententation

Web Server
:  A web server is a computer that runs websites. It's a computer program that distributes web pages as they are requisitioned. The basic objective of the web server is to store, process and deliver web pages to the users. This intercommunication is done using Hypertext Transfer Protocol (HTTP)

Express
:  its a wireframe for back end web application for Node. js, released as free and open-source software under the MIT License. It is designed for building web applications and APIs.
Routing

:  the process of selecting a path for traffic in a network or between or across multiple networks

WRRC
:  its the jerouny from the client to the server by sending requet by http and recieving responds from server

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
     * What is the node.js and why do we use it and what the difference between library and framework as express
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    * when to use TDD
    * HOW to use it 
    * what is the test unit 

## Preparation Materials
1. An introduction to NodeJS and Express
: Node is aprogramme that allows you to apply your j.s skills out side the chrome . it uses v8 (an engine to translate ). its helpful for asyn programmimg using an event loop
2. What is NPM
: its a node packages manger to help us install libraries frameworks in our project
3. What is TDD
: testing driven development its a software development that test the requirement before coding 
4. CI/CD
: CI its a contionus integration which mean less conflict through working on branches a
: CD its a contionus dilevery keep adding the changes to our live server.