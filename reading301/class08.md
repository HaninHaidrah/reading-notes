# APIs

## API Design Best Practices

1. What does REST stand for?

* REST stands for representational state transfer and was created by computer scientist Roy Fielding.

2.REST APIs are designed around a ____.

* REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

3.What is an identifer of a resource? Give an example.

* A resource has an identifier, which is a URI that uniquely identifies that resource
* Ex ![url](https://i.stack.imgur.com/mcTKf.jpg)

4.What are the most common HTTP verbs?

![image](https://19yw4b240vb03ws8qm25h366-wpengine.netdna-ssl.com/wp-content/uploads/Understanding-Idempotency-and-Safety-in-API-Design.png)

5.What should the URIs be based on? a version number

6.Give an example of a good URI.

![uri](https://joinup.ec.europa.eu/sites/default/files/inline-images/URI_Visualisation_v0_03.jpg)

7.What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

* Chatty API is one that requires consumer to make tremendous (subjective matter) amount of distinct API calls to get needed information about a resource. George Reese has defined chatty API as any API that requires consumer to do more than a single call to perform a single, common operation.

8.What status code does a successful GET request return?

 >2xx successful – the request was successfully received, understood, and accepted

9.What status code does an unsuccessful GET request return?

 >5xx server error – the server failed to fulfil an apparently valid request

10.What status code does a successful POST request return?

 >
11.What status code does a successful DELETE request return?

 >A successful response of DELETE requests SHOULD be HTTP response code 200 (OK) if the response includes an entity describing the status, 202 (Accepted) if the action has been queued, or 204 (No Content) if the action has been performed but the response does not include an entity
