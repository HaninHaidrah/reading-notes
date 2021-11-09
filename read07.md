# Reading: Bearer Authorization

## Review, Research, and Discussion

1. Write the following steps in the correct order:
    - Receive access token
    - Redirect to a third party authentication endpoint
    - Register your application to get a client_id and client_secret
    - Make a request to a third-party API endpoint
    - Ask the client if they want to sign in via a third party
    - Receive authorization code
    - Make a request to the access token endpoint
    

    **The Answer**
    1. Register your application to get a client_id and client_secret
    2. Ask the client if they want to sign in via a third party
    3. Redirect to a third party authentication endpoint
    4. Receive access token
    5. Make a request to the access token endpoint
    6. Receive authorization code
    7. Make a request to a third-party API endpoint

2. What can you do with an authorization code?
 - we implemented it to have more secure for users data like passwords 

3. What can you do with an access token?
  - we use token to avoid saving the secure data into the browser while the user go through the pages
  - we use it to anoid being directed to login page once the user want to refresh the page.

4.  What’s a benefit of using OAuth instead of your own basic authentication?    
  - the most important part is that generating token each time well inter the web application which means more secure


 ## DOCUMENTAION:

Client ID
:  At registration the client application is assigned a client ID and a client secret (password) by the authorization server
Client Secret
:  a secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors
Authentication Endpoint
:  Endpoint authentication is a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.
Access Token Endpoint
:  is an HTTP endpoint that micropub clients can use to obtain an access token given an authorization code.
API Endpoint
:  the code that allows two software programs to communicate with each other
Authorization Code
:   is a temporary code that the client will exchange for an access token
Access Token 
:  a proxy for auth data to avoid saving data on the browser


## PREVIEW: 
1. Which 3 things had you heard about previously and now have better clarity on?
   - more idea of auth
   - the differnauthentication and authorization.
   - how to implement auth code
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   - how to use token
   - the difference between bearer and basic auth
   - what's jwt
3. What are you most excited about trying to implement or see how it works?
   - bearer auth once we werent able to refresh the page we we were 301 and keep loging in

## Preparation Materials
1. JWTs Explained => JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
2. JWT is a very modern, simple and secure approach which extends for Json Web Tokens. Json Web Tokens are a stateless solution for authentication. So there is no need to store any session state on the server, which of course is perfect for restful APIs. Restful APIs should always be stateless, and the most widely used alternative to authentication with JWTs is to just store the user's log-in state on the server using sessions. But then of course does not follow the principle that says that restful APIs should be stateless and that's why solutions like JWT became popular and effective.