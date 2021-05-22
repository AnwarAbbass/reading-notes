# Review, Research, and Discussion
### - Explain what a “Singleton” is (in Computer Science terms)
*The Singleton design pattern is a creational pattern that states that one and only one instance of a class would persist in the memory during the application's life cycle. In other words, this design pattern restricts instantiation of a class to just one object.*

### - Explain how the Singleton pattern can be used with Node modules, specifically with classes

*We need singleton when we want to make sure there is only one object instantiated. Therefore, instead of creating a new object we need to ensure the constructor was called only once and then we reuse the instance. We can achieve this by refactoring our class to have: hidden (private) constructor.*


<br>


# Vocabulary Terms
## Router Middleware:

* Middleware is a piece of code that comes in the middle of request and response.
*Router is used to manage these incoming requests. It kind of routes your requests to correct handler/code .

## oDynamic Module Loading:

* Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.

## Singleton Pattern:

* singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance.

## CRUD -> REST Method Matches:

- CREATE -> POST
-READ -> GET
-UPDATE -> PUT
-DELETE -> delete

## Mock Testing:

* Mock testing is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. 

# Securing Passwords with Bcrypt Hashing Function

![](https://en.bitcoinwiki.org/upload/en/images/3/32/Bcrypt.png)

- Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.

- The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords. 

## PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM

- Brute Force attack
- Hash Collision attack
- BCrypt, IT's SLOW AND STRONG AS HELL

# Basic access authentication

![](https://techmonger.github.io/static/images/41/basic-access-authentication.png)

basic access authentication is a method for an HTTP user agent to provide a user name and password when making a request.

**note:**
*to install bcrypt run this command `npm i bcrypt`*

***how to use in vs***
```
const bcrypt = require('bcrypt');
const saltRounds = 10;
const myPlaintextPassword = 's0/\/\P4$$w0rD';
const someOtherPlaintextPassword = 'not_bacon';

bcrypt.hash(myPlaintextPassword, saltRounds, function(err, hash) {
    // Store hash in your password DB.
});
```