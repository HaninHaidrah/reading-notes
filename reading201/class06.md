

# Chapters

## Chapter3 Object Literals:

A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.

***The following demonstrates an example object literal:***

>var myObject = {  
    sProp: 'some string value',  
    numProp: 2,
    bProp: false
};


Object literal property values can be of any data type, including array literals, functions, and nested object literals. Here is another object literal example with these property types:

>var Swapper = {  
    // an array literal  
    images: ["smile.gif", "grim.gif", "frown.gif", "bomb.gif"],
    pos: { // nested object literal  
        x: 40,  
        y: 300  
    },  
    onSwap: function() { // function  
        // code here
    }
};  


* Object Literal Syntax  
*Object literals are defined using the following syntax rules:*

   * 1. A colon separates property name`[1]` from value.
   * 2. A comma separates each name-value pair from the next.
   * 3. A comma after the last name-value pair is optional.`[2]`


*If any of the syntax rules are broken, such as a missing comma or colon or curly brace, a JavaScript error will be triggered. Browser error messages are helpful in pointing out the general location of object literal syntax errors, but they will not necessarily be completely accurate in pointing out the nature of the error.*

* Why and How We Use Object Literals  
Several JavaScripts from dyn-web use object literals for setup purposes. Object literals enable us to write code that supports lots of features yet still provide a relatively straightforward process for implementers of our code. No need to invoke constructors directly or maintain the correct order of arguments passed to functions. Object literals are also useful for unobtrusive event handling; they can hold the data that would otherwise be passed in function calls from HTML event handler attributes.

![img](https://i.stack.imgur.com/o8aIx.png)



## Chapter5: Document Object Model  
Every web page resides inside a browser window which can be considered as an object.

A Document object represents the HTML document that is displayed in that window. The Document object has various properties that refer to other objects which allow access to and modification of document content.

* The way a document content is accessed and modified is called the Document Object Model, or DOM. The Objects are organized in a hierarchy. This hierarchical structure applies to the organization of objects in a Web document.

    1. Window object − Top of the hierarchy. It is the outmost element of the object hierarchy.

    2. Document object − Each HTML document that gets loaded into a window becomes a document object. The document contains the contents of the page.

    3. Form object − Everything enclosed in the <form>...</form> tags sets the form object.

    4. Form control elements − The form object contains all the elements defined for that object such as text fields, buttons, radio buttons, and checkboxes.

Here is a simple hierarchy of a few important objects −
![img](https://www.tutorialspoint.com/javascript/images/html-dom.jpg)

***HTML DOM***   
There are several DOMs in existence. The following sections explain each of these DOMs in detail and describe how you can use them to access and modify document content.

1. The Legacy DOM − This is the model which was introduced in early versions of JavaScript language. It is well supported by all browsers, but allows access only to certain key portions of documents, such as forms, form elements, and images.

2. The W3C DOM − This document object model allows access and modification of all document content and is standardized by the World Wide Web Consortium (W3C). This model is supported by almost all the modern browsers.

3. The IE4 DOM − This document object model was introduced in Version 4 of Microsoft's Internet Explorer browser. IE 5 and later versions include support for most basic W3C DOM features.

***DOM compatibility***  

If you want to write a script with the flexibility to use either W3C DOM or IE 4 DOM depending on their availability, then you can use a capability-testing approach that first checks for the existence of a method or property to determine whether the browser has the capability you desire. For example −

>if (document.getElementById) {  
   // If the W3C method exists, use it  
} else if (document.all) {  
   // If the all[] array exists, use it  
} else {  
   // Otherwise use the legacy DOM  
}  