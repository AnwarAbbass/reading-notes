# The Call Stack

A call stack is a mechanism which track with function is currently being run and what functions are called from within that function. _It can only do one thing at a time(single-threaded)_.

- The compiler adds the finction called to the call set and then begins performing the function.
- Any other functions called by this function are added to the call stack.
- The compiler pulls it out when the current job ends.
- The "Stack Overflow" error caused when the stack takes more space than it is assigned to .

![](https://i.stack.imgur.com/xAQPR.png)

# Debugging:

- The easiest and most common way its to debug JS code it is by using `console.log()` and see the result in the incpect or trminal.

## Types of error messages

1. Reference errors.
2. Syntax errors.
3. Range errors.
4. Type errors
