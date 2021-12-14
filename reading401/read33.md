# Reading: <Login /> and <Auth />
## Review, Research, and Discussion

1. Why is the Context API useful?
    - The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux
2. Can a component outside of a provider get its context?
   - No, you can't. The only way to update context it would be change the value sent to the Context. Provider. React context is available only when the UI is available
3. What are some common use cases for using the Context API?
    - Theming — Pass down app theme.
    -  Pass down translation messages.
    - Authentication — Pass down current authenticated user
4. Describe “Context Hell”
   - Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API. 

 ## Documentation 
global state
:  Its a state which can be shared between all components and edit them

global context
:  its the compononent where can we store our state that could be global

provider
:  component can be connected to the store, most applications will render a <Provider> at the top level, with the entire app's component tree inside of it.

consumer  
:  A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component. Requires a function as a child. The function receives the current context value and returns a React node.

## Review :

**DEFINITION OF ROLE-BASED ACCESS CONTROL (RBAC)**
   - Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.
   
**BENEFITS OF RBAC**
Managing and auditing network access is essential to information security. Access can and should be granted on a need-to-know basis. With hundreds or thousands of employees, security is more easily maintained by limiting unnecessary access to sensitive information based on each user’s established role within the organization. Other advantages include: