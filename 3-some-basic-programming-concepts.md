Let's talk about some basic concepts you will always face as a programmer :

## Functions Prototype
In computer programming, a function prototype or function interface refers to the definition or declaration of a function. In the prototype of a function, you'll always find :
- The name of the function
- The list of arguments or inputs that takes the function, with their type
- The type of the value that returns the function

Consider the following function prototype in c:
```
int sum( int a, int b );
```
By reading the protype of this function, we know that the function is called `sum`. It takes 2 inputs or arguments : `a` and `b`. These two arguments are integers. The value returns by this function is also an integer : `int sum...`

### The importance of a prototype
When you read a documentation about a programming language, most of the time, you'll have to read the prototype of the functions used in this programming language. When you know how to read the informations that the prototypes tell you, you'll know how to use the functions.

## Syntaxtic sugar
Syntaxtic sugar are syntaxes in programming languages that are designed to make things easier to read or to express.

Syntaxtic sugar make the expressions shorter or more concise.

Let say you have a variable called "counter", and you want to add 1 to this variable, the basic way to do this is like below:
```
counter = counter + 1
```
There are also orther ways to express that. We call these orther syntaxes `syntaxtic sugar` :
1. `counter += 1`
2. `counter++`
3. `++counter`

## Logical Expressions vs Logical Operators

### Logical Expressions
A logical expression is a statement that can be evaluated to true or false. By example, `a < b` is a logical expression that verifies if `a` is less than `b`. The result of this expression will be `true` if `a` is effectively less than `b`. It will be `false` ortherwise, (i.e if `a` is more than or equal to `b`).

### Logical Operators
Logical operators are operators we use to make logical expressions. Most of the time, they are operators we use to compare values.

By example, in the expression : `a < b`, the symbol `<` is a logical operator. It is the symbol used used to compare the value `a` to `b`.

Here is a list of the most used logical operators :
- `==` used to compare if two values are equal
- `<` used to verify if a value is less then another one
- `>` used to verify if a value is more than another one
- `<=` used to verify if a value is less or equal to another one
- `>=` used to verify if a value is more or equal to another one

## How to evaluate the quality of a code
What one individual values as top quality code may be drastically different from what another individual values. That means that the quality of a code can depend on the needs of the team working on the project, the problem that the code solves or the programming language you use. But when we evaluate the quality of a code, there are three main aspects we have to always consider :  
  
1. CORRECTNESS  
  
A top quality code has to always do exactly what it is written for. It has to solve exactly the problem you have.  
  
2. DESIGN  
  
This refers to how well written the code is. It has to be readable, easy to understand. This is why the use of some common design patterns are useful.  
  
3. THE STYLE  
  
This refers to how well formatted the code is. Here, we talk about the indentation, the convention used to name the files, the variables, the functions, etc... The overall project have to respect the same style. 
