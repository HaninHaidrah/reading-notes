# Reading: useState() Hook
## Review, Research, and Discussion
* In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

1. How does React differ from vanilla JS/HTML/CSS?
    - Event handling in HTML and React are different from one another in terms of syntax and some rules. The reason behind this is that React works on the concept of virtual DOM, on the other hand, the HTML has access to the Real DOM all the time
2. What is the primary difference between a function component and a class component?
    - A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components

 ## DOCUMENTATION : 
 Functional Components
 :  A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element.

Children / Child Components   
:  Children allow you to pass components as data to other components, just like any other prop you use. ... The special thing about children is that React provides support through its ReactElement API and JSX. XML children translate perfectly to React children

## Review :

**Why Hooks?** [source](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

- We know that components and top-down data flow help us organize a large UI into small, independent, reusable pieces. However, we often can’t break complex components down any further because the logic is stateful and can’t be extracted to a function or another component. Sometimes that’s what people mean when they say React doesn’t let them “separate concerns.”

- These cases are very common and include animations, form handling, connecting to external data sources, and many other things we want to do from our components. When we try to solve these use cases with components alone, we usually end up with:
   - Huge components that are hard to refactor and test.
    Duplicated logic between different components and lifecycle methods.