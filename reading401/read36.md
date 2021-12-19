# Reading: Application State with Redux

## Review, Research, and Discussion
1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”
   - Local Storage is available for every page and remains even when the web browser is closed, but you cannot read it on the server. The stored data has no expiration date in local storage. ... Local Storage is for client side, whereas cookies are for the client as well as server side.
2. Explain 3rd party cookies.
    - Third-party cookies are created by domains that are not the website (or domain) that you are visiting. These are usually used for online-advertising purposes and placed on a website through adding scripts or tags. A third-party cookie is accessible on any website that loads the third-party server's code.
3. How do pixel tags work?
    - A tracking pixel (also called 1x1 pixel or pixel tag) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. ... The tracking pixel URL is the memory location on the server. When the user visits a website, the image with the tag is loaded from this server.

 ## Documentation :
 cookies
 :  Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

authorization
:  the act of authorizing. permission or power granted by an authority; sanction.


access control
:  Access control is a fundamental component of data security that dictates who's allowed to access and use company information and resources.

conditional rendering  
:   Conditional rendering is a term to describe the ability to render different user interface (UI) markup if a condition is true or false


## Preview
* What is Redux? Redux is a predictable state container designed to help you write JavaScript apps that behave consistently across client, server, and native environments and are easy to test. While it's mostly used as a state management tool with React, you can use it with any other JavaScript framework or library.

![img](https://miro.medium.com/max/919/1*EdiFUfbTNmk_IxFDNqokqg.png)

* Is Redux necessary?
Even though Redux is a great tool for state management, it's important not to overuse it. ... You might not need Redux if your app state management: Implies simple UI changes that follow plain logic. Handles data that comes from a single source per view and there is no or little risk of having data inconsistency bug