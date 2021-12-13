# Reading: Context API - Behaviors

## Review, Research, and Discussion
1. When you have multiple contexts, what component type should you use (class/function) and why?
    - To keep context re-rendering fast, React needs to make each context consumer a separate node in the tree. If two or more context values are often used together, you might want to consider creating your own render prop component that provides both.

2. What are some good use cases for using the Context API for global state?
    - Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context
3. How can you best test context?
     - The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing

## Documentation:
context
:  Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component: class App extends React.


useContext()
:  useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level.

static context
:  react can calculate default props without needing to mount your component

## Preview: 

* Context: 
  - In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

* What is a hook and context?
  - The hook is called with the context as an argument and returns the user name value. <Layout /> and <Header /> intermediate components don't have to pass down the userName prop. That is the great benefit of the context: it removes the burden of passing down data through the intermediate components.

  ![img](https://dmitripavlutin.com/90649ae4bdf379c482ad24e0dd220bc4/react-context-3.svg)
