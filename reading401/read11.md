# Readings: Event Driven Applications

## Review, Research, and Discussion
1. Why is access control important? 
    - to give a certain permissions to the role so it identifies the rigth permission and action
2. Describe an application that would need access control.
     - for example an app for students and teachers like canvas , not all of us can do the same thing ,the students are different from the ta and from the instructor
3. What is a role used for?
     - it uses to give the right permission and according to that invoke the right method.
4. Why is role based access control more scalable than discretionary or mandatory access control?
    - because the role can be changes easily , i think


## DOCUMENTATION: 
Authorization
:  Authorization is the process of giving someone permission to do or have something. Thus, authorization is sometimes seen as both the preliminary setting up of permissions by a system administrator and the actual checking of the permission values that have been set up when a user is getting access 

Role Based Access Control
:  Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network

Capabilities
:  the actions that related to each role 


## Preview
1. Which 3 things had you heard about previously and now have better clarity on?
   - the idead behind creating auth app
   - how to add more security 
   - understanding some terms clearly.
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   - whats the event app
   - how implement it
   - what's the difference between on and ommit methods

* Event-Driven Programming => is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision. In this article we’re going to go over how Event-Driven Programming works and how we can make the best use of it in our Node.js projects.

* EventEmitter
Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challange, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.

* how to access it=>  We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.