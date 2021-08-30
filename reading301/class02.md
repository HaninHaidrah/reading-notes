##  State and Props

### Questions about React lifecycle:
1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?  
*componentDidMount will only be called once after the first render*
2. What is the very first thing to happen in the lifecycle of React?
*The  ***Constructor*** is the first React lifecycle *
3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
    1. Constructor
    2. React Updates
    3. render
    4. componentDidMount 
    5. componentWillMoun
4. What does componentDidMount do?
*This method is invoked immediately after a component is mounted*

### Questions about React State Vs Props:
1. What types of things can you pass in the props?
* any types of date you can pass strings,numbers,functions anything*
2. What is the big difference between props and state?
*props you passed into compononats (ouside) but ***state** inside the compnonts*
3. When do we re-render our application?
*React components automatically re-render whenever there is a change in their state or props*
4. What are some examples of things that we could store in state?
*Your data (the value of the counter) is stored within the App component, and can be passed down its children.*