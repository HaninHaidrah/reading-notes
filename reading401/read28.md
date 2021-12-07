# Reading: Component Lifecycle / useEffect() Hook
 
 ## Review, Research, and Discussion
1. Why do we not need more .html pages in a multi-page React app?
     - js from where your entire web-app is loaded in fragments and components. This behaviour of rendering components and pages on a single page and changing the DOM( is a single page behaviour and hence the name), instead of loading a new page with new content, this makes it feel like a single application
2. If we wanted a component to show up on every page, where would we put it and why?
    - Outside the <BrowserRouter/>
    - Inside the <BrowserRouter />, outside a <Route />
    - Inside a <Route />
         - I think Inside the <BrowserRouter />, outside a <Route />

3. What does routing do with the components that were rendered when a new route is requested
     - pass the component prop an inline function. When you use component, the router uses React. createElement to create a new React element from the given component. That means if you provide an inline function to the component prop, you would create a new component every render.

4. What does props.children contain?
    - props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a componen
5. How do useState() and this.setState() differ?
    - the setState method found in class components, useState does not automatically merge update objects.,setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state.

## Documentation:
State Hook
:  Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We'll learn other Hooks later. 

Mounting and Un-Mounting
:  React does so by "mounting" (adding nodes to the DOM), "unmounting" (removing them from the DOM), and "updating" (making changes to nodes already in the DOM).

## Preview:

**Hooks** =>  are a new addition in React 16.8. They let you use state and other React features without writing a class.

**What is use effect**?
- useEffect is a hook for encapsulating code that has 'side effects,' and is like a combination of componentDidMount , componentDidUpdate , and componentWillUnmount . Previously, functional components didn't have access to the component life cycle, but with useEffect you can tap into it

