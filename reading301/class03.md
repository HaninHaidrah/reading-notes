#  Passing Functions as Props:
## Questions about 
1. What does .map() return?
* map() function returns a map object(which is an iterator) of the results after applying the given function to each item of a given iterable (list, tuple etc.)  
[map](https://i.stack.imgur.com/TysBm.png)


2. If I want to loop through an array and display each value in JSX, how do I do that in React?

* .map() in JavaScript iterates through an array and calls a specified function for each of the items. Components in JSX are JS functions. For each object in the array, a block of JSX elements is returned.

Also, data from the object is passed to each block using the JSX handlebars-like curly brackets. 

3. Each list item needs a unique ____.
* “map only unique values javascript”  
(code)[https://www.codegrepper.com/codeimages/javascript-map-distinct-value-from-object.png]
4. What is the purpose of a key?
*The keys in Map are ordered in a simple, straightforward way: A Map object iterates entries, keys, and values in the order of entry insertion.*



## Questiona about The Spread Operator:
1. What is the spread operator?
2. List 4 things that the spread operator can do.
3. Give an example of using the spread operator to combine two arrays.
4. Give an example of using the spread operator to add a new item to an array.
5. Give an example of using the spread operator to combine two objects into one.

***The Answers:***:
Spread syntax (...) allows an iterable such as an array expression or string to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected, or an object expression to be expanded in places where zero or more key-value pairs (for object literals) are expected. 
1. Copying an array.
2. Concatenating or combining arrays.
3. Using Math functions.
4. Using an array as arguments.
(code)[https://samanthaming.gumlet.io/tidbits/14-combine-multiple-arrays-using-spread.jpg.gz]
(code)[https://miro.medium.com/max/1400/1*ck6Fs5k54T8Yv09D2dS0jA.png]


## Questions about How to Pass Functions Between Components:
1. In the video, what is the first step that the developer does to pass functions between components?
2. In your own words, what does the increment function do?
3. How can you pass a method from a parent component into a child component?
4. How does the child component invoke a method that was passed to it from a parent component?
***The Answers***:
The Increment( ) function determines the next node at the same level. You can also increase the level of a node by one at a specified level.

* 1. import React from "react";export default function Child({data, onChildClick}) { return ( <div className="child"> ...
  2. import Child from './Child'
  3. import React from "react"; import "./styles.css";

#### How to invoke :

* Create a boolean variable in the state in the parent class. Update this when you want to call a function. Create a prop variable and assign the boolean variable. From the child component access that variable using props and execute the method you want by having an if condition.

