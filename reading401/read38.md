# Readings: Redux - Asynchronous Actions

## Review, Research, and Discussion
1. How granular should your reducers be?
    -  focus on more complex or unusual interactions which differ from the default of “update of this input means update of that property in the state
3. named action is dispatched
    -  dispatch is used as a callback which gets invoked once some async action is complete. In redux-thunk dispatch is simply a function which dispatches an action to the Redux store
4. Name a strategy for preventing the above
   - use middlewares
## Document the following Vocabulary Terms
store
:  A store is an immutable object tree in Redux. A store is a state container which holds the application's state.

combined reducers
:  unction turns an object whose values are different reducing functions into a single reducing function you can pass to createStore

## Review :
- Redux Thunk

    **Thunk middleware for Redux. It allows writing functions with logic inside that can interact with a Redux store's dispatch and getState methods.**

   - How redux work : ![img](https://d33wubrfki0l68.cloudfront.net/08d01ed85246d3ece01963408572f3f6dfb49d41/4bc12/assets/images/reduxasyncdataflowdiagram-d97ff38a0f4da0f327163170ccc13e80.gif) 


   - Why we use middleware as thunk:
   
   **Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store**