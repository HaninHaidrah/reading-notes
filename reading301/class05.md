## Questions about React Docs - thinking in React  


!(code)[https://bestof.nyc3.digitaloceanspaces.com/react/react-thinking-in-react-hooks.jpeg]


1. How would you break a mock into a component heirarchy?  
* The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components!

* But how do you know what should be its own component? Use single responsibility principle , a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.  

2. What is the single responsibility principle and how does it apply to components?  
* The single-responsibility principle (SRP) is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part. All of that module, class or function's services should be narrowly aligned with that responsibility.  


!(code)[https://miro.medium.com/max/1400/1*UY-BQhUAfNciHI1iAHfwXg.png]

3. What does it mean to build a ‘static’ version of your application?  
* What is a Static App?
Static applications and websites render in the user’s browser without the need for server side processing, this means that all the rendering of HTML, CSS, and JavaScript is done on the client side, rather then relying on server side technologies.   

4. Once you have a static application, what do you need to add?  
* Deploy it
5. What are the three questions you can ask to determine if something is state?  
   1. Is it passed in from a parent via props? If so, it probably isn’t state.
   2. Does it remain unchanged over time? If so, it probably isn’t state.
   3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

6. How can you identify where state needs to live?   
* To know where is it exactly 
  1. Identify every component that renders something based on that state.
  2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
  3. Either the common owner or another component higher up in the hierarchy should own the state.
  4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
