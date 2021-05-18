# Review, Research, and Discussion
1. Name 3 real world use cases where you’d want to change the request with custom middleware:
    1. authentication
    2. parameters validation
    2. Error Handing Middleware

1. At what point in the request lifecycle can you “inject” middleware?
will execute whenever a request to the server has been made

# Clases
Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.
<br>

`class Rectangle {`<br>
  `constructor(height, width) {`<br>
    `this.height = height;`<br>
    `this.width = width;`<br>
  `}`<br>
`}`<br>

<br>

# Routing
Routing refers to how an application’s endpoints (URIs) respond to client requests.

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests, you can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function.

| Method             | Description                                                                           |
| ------------------ | ------------------------------------------------------------------------------------- |
| `res.download()`   | Prompt a file to be downloaded.                                                       |
| `res.end()`        | End the response process.                                                             |
| `res.json()`       | Send a JSON response.                                                                 |
| `res.jsonp()`      | Send a JSON response with JSONP support.                                              |
| `res.redirect()`   | Redirect a request.                                                                   |
| `res.render()`     | Render a view template.                                                               |
| `res.send()`       | Send a response of various types.                                                     |
| `res.sendFile()`   | Send a file as an octet stream.                                                       |
| `res.sendStatus()` | Set the response status code and send its string representation as the response body. |
