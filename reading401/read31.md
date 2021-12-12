# Reading: Context API

## Review, Research, and Discussion
1. Describe use cases useState() vs useReducer(): 
   - when there are a  lot of states.
   
2. Why do custom hooks need the use prefix?
   - This is mainly to have an extra option for sharing state and logic between components. ... Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.
3. What do custom hooks usually do?
  - Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.
4. Using any list of custom hooks, research and name one that you think will be useful in your applications
   - use state ()Instead, always use Hooks at the top level of your React function, before any early returns. By following this rule, you ensure that Hooks are called in the same order each time a component renders. That's what allows React to correctly preserve the state of Hooks between multiple useState and useEffect calls.
5. Describe how a hook that fetches API data might work
   - Put the fetchData function above in the useEffect hook and call it, like so:
   > useEffect(() => { const url = "https://api.adviceslip.com/advice"; const fetchData = async () => { try { const response = await fetch(url); const json = await response. json(); console. log(json); } catch (error) { console.

## DOCUMENTATION : 
reducer
: a pure function that takes an action and the previous state of the application and returns the new state

## Preview: 

* Context provides=>  a way to pass data through the component tree without having to pass props down manually at every level.

* In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.


* when =>  When to Use Context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.