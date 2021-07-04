# Chapter 2 and 10
## *Text And intro to Css*
1. Headings and paragraphs
2. Bold, Itlatic and emphasis
3. Structral and symantic Markup


### Headings and paragraphing:
- we have 6 headings numbered as their importance:
    * `<h1>` standing for the most imprtant headings 
    * `<h6>` standing for the least important ones.


![pic](https://qph.fs.quoracdn.net/main-qimg-6a92817c1dc99bf922087ea984587c3c.webp)

- we have a tag which stands for paragraph *`<p>`*


### Bold ,Itlatic and emphisis
 #### Dictionary :
1. `<b>` 

| Code                                                                            | purpose                            |
| -----------                                                                     | -----------                        |
|`<b>`                                                                            | bold                               | 
|`<i>`                                                                            | itlatic                            |  
|`<sup>`                                                                          | character as number ,dates         |
|`<sub>`                                                                          | characters s foot notes or chemical| 
|`<br>`                                                                           | line break inside                  |
|`<hr>`                                                                           | line between themes                |
|`<srong>`                                                                        |important element                   |


### introducing Css:
- Cascading Style Sheets, fondly referred to as CSS, is a simply designed language intended to simplify the process of making web pages presentable. CSS allows you to apply styles to web pages. More importantly, CSS enables you to do this independent of the HTML that makes up each web page.
  - CSS is easy to learn and understood, but it provides powerful       control over the presentation of an HTML document.
    - The selector points to the HTML element you want t
  - The declaration block contains one or more declarations separated by semicolons.
    Each declaration includes a CSS property name and a value, separated by a colon.
    For Example:
  * –; color is property and blue is value.
  * –; font size is property and 12px is value.

A CSS declaration always ends with a semicolon, and declaration blocks are surrounded by curly braces.


### J.S 
 * JavaScript ("JS" for short) is a full-fledged dynamic programming language that can add interactivity to a website. It was invented by Brendan Eich (co-founder of the Mozilla project, the Mozilla Foundation, and the Mozilla Corporation).

* JavaScript is versatile and beginner-friendly. With more experience, you'll be able to create games, animated 2D and 3D graphics, comprehensive database-driven apps, and much more!

* JavaScript itself is relatively compact, yet very flexible. Developers have written a variety of tools on top of the core JavaScript language, unlocking a vast amount of functionality with minimum effort. These include:

* Browser Application Programming Interfaces (APIs) built into web browsers, providing functionality such as dynamically creating HTML and setting CSS styles; collecting and manipulating a video stream from a user's webcam, or generating 3D graphics and audio samples.
Third-party APIs that allow developers to incorporate functionality in sites from other content providers, such as Twitter or Facebook.
Third-party frameworks and libraries that you can apply to HTML to accelerate the work of building sites and applications.
It's outside the scope of this article—as a light introduction to JavaScript—to present the details of how the core JavaScript language is different from the tools listed above. You can learn more in MDN's JavaScript learning area, as well as in other parts of MDN.

* The section below introduces some aspects of the core language and offers an opportunity to play with a few browser API features too. Have fun!


### Decisions and Loops:


here are situations when we want to run the code at different conditions, such as, if one condition applies run a particular code, if another condition applies another code is run. This is prioritized with "if" and "else if" conditionals as follows:

     < `function getColor(phrase){
       if (phrase === "stop"){
       console.log("red");
       } else if (phrase === "slow"){
       console.log("yellow");
       } else if (phrase === "go"){
       console.log("green");
      } else {
       console.log("purple");
       }
       }`