# Component Composition
## Review, Research, and Discussion

* Can a parent component access the state of a child component?
  * yes by using React.createRef().
  
* What can be passed along in a prop variable?
  * Any information, function, JavaScript that needs to be passed. 

* How can a child component “know” the state of another component?
  * pass the component's state to it's child components as props.



## Vocabulary Terms

### component props :
  * a keyword in React stands for `properties`, can be any information that needs to be passed to another component.

### component state :
  * The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component.


### application state :
  * is interface between data and the representation of this data with UI elements on the front-end. State is able to keep the data of different components in sync because each state update will rerender all relevant components.




## react basics recap

 * The Component Lifecycle : it details the life of a component, components are born, do some things , and then they die.

* A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM.
* Higher-Order Components: is a function that takes a component and returns a new component.

* Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.
* You can think of React lifecycle methods as the series of events that happen from the birth of a React component to its death.
* `setState()` in only these React lifecycle methods: `componentDidMount` , `componentDidUpdate` and `componentWillReceiveProps` .


## Components and Props

![](https://www.gatsbyjs.com/static/c058cc46416d6b9d5d27e571c885c936/6569d/component-with-props.png)


* Components let you split the UI into independent, reusable pieces, and think about each piece in isolation
* Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.
* Components can refer to other components in their output
* Whether you declare a component as a function or a class, it must never modify its own props
* All React components must act like pure functions (do not attempt to change their inputs and always return the same result for the same inputs) with respect to their props

## props.children
* we use `props.children` on components that represent ‘generic boxes’ and that ‘don’t know their children ahead of time’.

## Component Composition

![](https://res.cloudinary.com/practicaldev/image/fetch/s--yV_Dmfcz--/c_imagga_scale,f_auto,fl_progressive,h_500,q_auto,w_1000/https://cl.ly/21e6473eebb8/Image%252525202019-05-03%25252520at%252525205.30.33%25252520PM.png)

* Props and composition give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way.
* Pass a function when you can to update state multiple times.

## React Testing

* syep 1 
```
// import dependencies
import React from 'react'

// import API mocking utilities from Mock Service Worker
import { rest } from 'msw'
import { setupServer } from 'msw/node'

// import react-testing methods
import { render, fireEvent, waitFor, screen } from '@testing-library/react'

// add custom jest matchers from jest-dom
import '@testing-library/jest-dom/extend-expect'
// the component to test
import Fetch from '../fetch'
```
* step 2 
```
// declare which API requests to mock
const server = setupServer(
  // capture "GET /greeting" requests
  rest.get('/greeting', (req, res, ctx) => {
    // respond using a mocked JSON body
    return res(ctx.json({ greeting: 'hello there' }))
  })
)

// establish API mocking before all tests
beforeAll(() => server.listen())
// reset any request handlers that are declared as a part of our tests
// (i.e. for testing one-time error scenarios)
afterEach(() => server.resetHandlers())
// clean up once the tests are done
afterAll(() => server.close())

// ...
```

* step 3
```
test('handlers server error', async () => {
  server.use(
    // override the initial "GET /greeting" request handler
    // to return a 500 Server Error
    rest.get('/greeting', (req, res, ctx) => {
      return res(ctx.status(500))
    })
  )
  
  ```

