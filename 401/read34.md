# `<Login />` and `<Auth />`

## Review, Research, and Discussion
- Why is the Context API useful?
  * The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on.

- Can a component outside of a provider get its context? 
   - No 

- What are some common use cases for using the Context API?

   - when some data needs to be accessible by many components at different nesting levels

- “Context Hell”
  - the React Context hell is the nasty code you get taking advantage of the React Context API.

## Vocabulary Terms

|Term  | hhhh|
|-------|-----|
|global state| Context provides a way to pass data through the component tree without having to pass props down manually at every level|
|global context|context that is applied to all components inside your code|
|provider|React component that allows consuming components to subscribe to context changes.|
|consumer |React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component​.|
------
## role-based access control
---
![](https://www.dnsstuff.com/wp-content/uploads/2019/10/role-based-access-control.jpg)

----------
## react-cookies
***Cookies*** are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites

- to install it 
```
npm install react-cookies --save
```
- example  on react cookies
```
import cookie from 'react-cookies'
cookie.save('userId', userId, { path: '/' })
cookie.load('token')
cookie.remove('userId', { path: '/' })
```
- To be able to access user cookies while doing server-rendering, you can use `plugToRequest` or `setRawCookie`

- `<CookiesProvider />` : to set the user cookies... On the server, the cookies props must be set using req.universalCookies or new Cookie(cookieHeader)

-`useCookies([dependencies])`: Access and modify cookies using React hooks