
## Array.map()

The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.


```js
const array1 = [1, 4, 9, 16];

// pass a function to map
const map1 = array1.map(x => x * 2);

console.log(map1);
// expected output: Array [2, 8, 18, 32]
```

***

## Array.reduce() 

The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.


```js
const array1 = [1, 2, 3, 4];
const reducer = (accumulator, currentValue) => accumulator + currentValue;

// 1 + 2 + 3 + 4
console.log(array1.reduce(reducer));
// expected output: 10

// 5 + 1 + 2 + 3 + 4
console.log(array1.reduce(reducer, 5));
// expected output: 15
```
***

## superagent()

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. works with Node. js.

```js
 request
   .post('/api/pet')
   .send({ name: 'Manny', species: 'cat' })
   .set('X-API-Key', 'foobar')
   .set('Accept', 'application/json')
   .then(res => {
      alert('yay got ' + JSON.stringify(res.body));
   });
```
A request can be initiated by invoking the appropriate method on the request object, then calling .then() (or .end() or await) to send the request. For example:

.then :
```
 request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });
```
await :


```
// pattern: https?+unix://SOCKET_PATH/REQUEST_PATH
//          Use `%2F` as `/` in SOCKET_PATH
try {
  const res = await request
    .get('http+unix://%2Fabsolute%2Fpath%2Fto%2Funix.sock/search');
  // res.body, res.headers, res.status
} catch(err) {
  // err.message, err.response
}
```

***

## Promise

The Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.

A Promise is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action's eventual success value or failure reason. This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future.

<br>

![](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/promises.png)

A Promise is in one of these states:

pending: initial state, neither fulfilled nor rejected.
fulfilled: meaning that the operation was completed successfully.
rejected: meaning that the operation failed.


Chained Promises
The methods promise.then(), promise.catch(), and promise.finally() are used to associate further action with a promise that becomes settled.


# How to Solve Programming Problems

1. Read the problem completely twice.
1. Solve the problem manually with 3 sets of sample data.
1. Optimize the manual steps.
1. Write the manual steps as comments or pseudo-code.
1. Replace the comments or pseudo-code with real code.
1. Optimize the real code.

---

# How to think like a programmer — lessons in problem solving

- Understand

- Plan

- Divide

- Stuck
