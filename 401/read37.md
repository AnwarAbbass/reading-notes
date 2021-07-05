# Redux - Combined Reducers

## Review, Research, and Discussion


- Why choose Redux instead of the Context API for global state?

     - In a large scale application, Redux is a better way to control state.

- What is the purpose of a reducer?

   -  Process of giving someone the ability to access a resource.

- What does an action contain?

  - Object literals that tell the reducer what is being done to the app, and any data required for the update.

- Why do we need to copy the state in a reducer?
  - Reducers are not allowed to modify the existing state, instead they must make immutable updates by copying the existing state and making changes to the copied values.


## Vocabulary Terms

### immutable state :
  - cannot be modified after it is created.
### time travel in redux :
  - Time travel is the ability to move back and forth among the previous states of an application and view the results in real time.

### action creator :
  - function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function. 

### reducer :
  - Functions that take current state and an action as arguments, and return a new state result, (state, action) => newState.

### dispatch :
 - A store holds the whole state tree of the application, the only way to change the state inside it is to dispatch an action on it.

## Redux - Combined Reducers


- combineReducers: helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore .

```
import { combineReducers, createStore } from 'redux'

const rootReducer = combineReducers({
  theDefaultReducer,
  firstNamedReducer,
  secondNamedReducer
})
```

- The resulting reducer calls every child reducer, and gathers their results into a single state object.

- combineReducers will combine all the reducers passed to it into a single reducing function

