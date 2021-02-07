# Java Script

  word| meaning   
------|-------
javaScript | programming language of the web and in-time compile
variable  |   piece of memory that can contain a data value

----

<span style="color:gray;font-family:Papyrus; font-size:2em;"> WRITING A SCRIPT </span>

*Begin with the big picture of what you want to accomplish and split it into smaller measures.*

There are 3 steps to write a great script

1. First, the assignment you want to accomplish must be specified. You can think of this as a computer puzzle to solve.

2.  then using a flowchart. You can then write down individual steps that the computer needs to perform in order to complete each individual task 

3. Each of the steps needs to be written in a programming language(JavaScript) that the computer understands.

![](https://grapholite.com/Images/FlowChartImage1.png)

----
<span style="color:gray;font-family:Papyrus; font-size:2em;"> EXPRESSIONS
 </span>

An expression evaluates into (results in) a single value. Broadly speaking
there are two types of expressions. 

1. EXPRESSIONS THAT JUST ASSIGN A
VALUE TO A VARIABLE like `var color = 'red';`
1. EXPRESSIONS THAT USE TWO OR
MORE VALUES TO RETURN A
SINGLE VALUE like `var area = 3 * 2;`

<span style="color:gray;font-family:Papyrus; font-size:2em;"> OPERATORS </span>

operat| example
------|-------
ASSIGNMENT OPERATORS| `age=22`
ARITHMETIC OPERATORS| `4*5+7`
STRING OPERATORS | `name= "anwar"+"abbass`
COMPARISON OPERATORS | `buy = 3 < 5`
LOGICAL OPERATORS |`buy= (5 > 3) && (2 < 4)`

<span style="color:gray;font-family:Papyrus; font-size:2em;"> FUNCTION </span>

Function is a group of statement that are perform a task.
To declare a function you need to define function name, parenthesises (you can put inside them variable name if you need to reseve values) after add function keyword then between brackets `{ }` write the statements.To call your function put the function name and a parenthesises(inside parenthesises write values or variables if the function ask)


![](data:image/png;base64,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)


we use `return variable ;` in the end of the function to return values from the function