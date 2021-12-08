# Reading: Advanced State with Reducers
## Review, Research, and Discussion
1. How can we ensure that an effect hook runs only once?
   -  by adding an empty array as a second parameters
2. Can useState() update more than one state variable at the same time?
   - yes, we can have multiple states inside of a single component: call multiple times useState()

3. Is useState() synchronous?
    - useState and setState both are asynchronous. They do not update the state immediately but have queues that are used to update the state object. This is done to improve the performance of the rendering of React components

 ## Documentation : 
State Hook
: A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We'll learn other Hooks later

Component Lifecycle
: Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component's existence. ... Mounting: Mounting is the stage of rendering the JSX returned by the render method itself

## preview :

* What is useReducer for?
    - The useReducer hook is used for complex state manipulations and state transitions. ... useReducer is a React hook function that accepts a reducer function, and an initial state. const [state, dispatch] = useReducer(reducer, initialState);This hook function returns an array with 2 values.

* What is useReducer action?
    - useReducer returns an array that holds the current state value and a dispatch function, to which you can pass an action and later invoke. ... We dispatch action objects to that reducer only, whereas in Redux, the dispatch function sends the action object to the store.

* How does useReducer hook work?
    - useReducer is one of a handful of React hooks that shipped in React 16.7. 0. It accepts a reducer function with the application initial state, returns the current application state, then dispatches a function.