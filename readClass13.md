# Sending Form Data

The client (web browser) sends a request to the server using the HTTP protocol. The server answers the request using the same protocol. The data sends to the server from the forms; `<form>` element defines how the data will be sent(_the data always will sent as a list of key/value pairs_).

- The two most important attributes are **action** and **method**.

  - The action attribute defines where the data gets sent.

  - The method attribute defines how data is sent.

    - _GET method_: the data sent to the server is appended to the URL.
    - _POST method_: the data provided in the body of the HTTP request.

![](https://codebridgeplus.com/wp-content/uploads/11inf03.gif)
