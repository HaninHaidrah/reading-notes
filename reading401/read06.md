# Readings: Authentication

## Review, Research, and Discussion: 
1. Explain what a “Singleton” is (in Computer Science terms)
    * A singleton is a class that allows only a single instance of itself to be created and gives access to that  created instance. It contains static variables that can accommodate unique and private instances of itself.
2. Explain how the Singleton pattern can be used with Node modules, specifically with classes
     * We need singleton when we want to make sure there is only one object instantiated. Therefore, instead of creating a new object we need to ensure the constructor was called only once and then we reuse the instance.We can achieve this by refactoring our class to have:
         - hidden (private)constructor
         - public getInstance method that returns instance of the class
3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?


## DOCUMENTATION:
Router Middleware
:  Middleware. It is a piece of code that comes in the middle of request and response . It kind of hijacks your request so that you can do anything that you want with your request or response eg: Modify the data or call the next middleware

Dynamic Module Loading
:  Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.

Singleton Pattern
:  in software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.

CRUD -> REST Method Matches
:   CRUD is an acronym that comes from the world of computer programming and refers to the four functions that are considered necessary to implement a persistent storage application: create, read, update and delete

Mock Test
:  creating a fake version of an external or internal service that can stand in for the real one, helping your tests run more quickly and more reliably. When your implementation interacts with an object's properties, rather than its function or behavior, a mock can be used.


## Preview
- Securing Passwords=> Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords.

- Basic Auth=> The BA mechanism does not provide confidentiality protection for the transmitted credentials. They are merely encoded with Base64 in transit and not encrypted or hashed in any way. Therefore, basic authentication is typically used in conjunction with HTTPS to provide confidentiality.

- Authentication OWASP => is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

- Bcrybt => A library to help you hash passwords. by using some methods.

Because the BA field has to be sent in the header