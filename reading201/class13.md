

## “The Past, Present, and Future of Local Storage for Web Applications”  
This is about the advantageous differences between local storage and web application storage. The differences being that local storage have options of storing informations in the following manner:

1. The registry
2. INI files
3. XML files
4. Embeded databases
5. Own file format invention
6. Web applitions only option is to store data as cookies which have downsides:

** What is Web Storage?**  

The HTML5's web storage feature lets you store some information locally on the user's computer, similar to cookies, but it is faster and much better than cookies. However, web storage is no more secure than cookies. Please check out the tutorial on PHP cookies to learn more about cookies.

The information stored in the web storage isn't sent to the web server as opposed to the cookies where data sent to the server with every request. Also, where cookies let you store a small amount of data (nearly 4KB), the web storage allows you to store up to 5MB of data.

There are two types of web storage, which differ in scope and lifetime:

1. Local storage — The local storage uses the localStorage object to store data for your entire website on a permanent basis. That means the stored local data will be available on the next day, the next week, or the next year unless you remove it.
2. Session storage — The session storage uses the sessionStorage object to store data on a temporary basis, for a single browser window or tab. The data disappears when session ends i.e. when the user closes that browser window or tab.

![img](https://i.stack.imgur.com/cI5kT.jpg)

**What is HTML5 storage?**

![img](https://sites.google.com/site/azswiki/_/rsrc/1286362842741/html5-localstorage/localstorage_browser_support.jpg)

* 1. IE 8.0+
* 2. Firefox 3.5+
* 3. Safari 4.0+
* 4. Chrome 4.0+
* 5. Opera 10.5+
* 6. Iphone 2.0+ 
* 7. Android 2.0+

***HTML5***
![img](https://clementbuchanan.github.io/reading-notes/images/html5.jpg)
*The future of HTML5*  

Currenly the future looks good for HTML5 but there is more to life than “5 megabytes of named key/value pairs,” and the future of persistent local storage and there are competing visions. One vision is SQL. In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This influenced the creation of the Web SQL Database. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to store code from JavaScript.