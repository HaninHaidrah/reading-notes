# Status Codes Based On REST Methods

![img](https://1.bp.blogspot.com/-NES44rDk7aY/XpsSeVDaRdI/AAAAAAAAHqc/BQ4NIgGXBtEVmilZbvazluMNAd06L5o6wCLcBGAsYHQ/s1600/api-list.PNG)

1. In your own words, describe what each group of status code represents:
  1.100’s = its a status which tells the client information about the header of the code may be his request will not be successful before sending a data.
  2.200’s = it tells the client his request is successul
  3.300’s = it tells that the resource isnt available now anymore
  4.400’s = it tells that there is an error but related to the request from the clint
  5.500’s = it tells there is an error in the server

2.What is a status code 202? it means that the request met all validation requirements at the time of sending.

3.What is a status code 308? This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

4.What code would you use if an update didn’t return data to a client? 204 No Content

5.What code would you use if a resource used to exist but no longer does? 307 Temporary Redirect

6.What is the ‘Forbidden’ status code? The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

* because we will use something is not localhost
2.What is middleware?

* Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system.

3.What does app.use(express.json()) do?

* express. json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app.

4.What does the /:id mean in a route?

* The req. params property is an object containing properties mapped to the named route “parameters”.

5.What is the difference beween PUT and PATCH?

* The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

6.How do you make a defalut value in a schema?

* Make mongoose string schema type default value as blank and make the field optional.
     >testschema = mongoose. Schema({ name:{ type:String, required:true, unique:true }, image:{ type:String, required:true }, category:{ type:String }, });

7.What does a 500 error status code mean?

* The HyperText Transfer Protocol (HTTP) 500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.

8.What is the difference between a status 200 and a status 201?

* The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed. A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).
