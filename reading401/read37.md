# Readings: Redux - Combined Reducers
## Review, Research, and Discussion


1. Why choose Redux instead of the Context API for global state?
    -  Redux works around the idea of having a central state called a store. To change the state, a component has to dispatch an action. The action is then passed on to the reducer, which changes the state of our application
2. What is the purpose of a reducer?
    - A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.
3. What does an action contain?
     - an object consists of type and payload
   
4. Why do we need to copy the state in a reducer
   - If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.Reducers specify how the application's state changes in response to actions sent to the store. Regardless of the state management pattern, You need to change the state through reducers as actions are responsible fpr source of information for the store


 ## Documentation :
 immutable state
 :  mmutable state means its value cannot be changed once it's created. ... A mutable state allows us to modify already created data structures and change them whichever way we want.

time travel in redux
:  Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.

reducer
:  a reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action

dispatch  
:  dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. 

## Review:
* Using combineReducers
  - Core Concepts
      - The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

**Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.**