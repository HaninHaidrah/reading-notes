# Readings: Redux - Additional Topics
## Review, Research, and Discussion


1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
   - In Redux, all your application state is held in the store; which is an object that holds the complete state tree of your app. There is only one way to change its state and that is by dispatching actions. Actions are objects that consist of a type and a payload property. They are created and dispatched by special functions called action creators. see a small contrived and detailed example below: by creating the Redux store
2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
   - applyMiddleware function as the third argument to the createStore() method. import { createStore, applyMiddleware from 'redux'


 ## Document the following Vocabulary Terms
middleware
:   action creators that return a function instead of an action object. That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the function's body once the asynchronous operations have been completed.

thunk 
:   k is a middleware that allows you to call the action creators that return a function(thunk) which takes the store's dispatch method as the argument and which is afterwards used to dispatch the synchronous action after the API or side effects has been finished.

## Review: 
*Purpose​ of The Redux Toolkit* :
 **The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:**

1. "Configuring a Redux store is too complicated"
2. "I have to add a lot of packages to get Redux to do anything useful"
3. "Redux requires too much boilerplate code"