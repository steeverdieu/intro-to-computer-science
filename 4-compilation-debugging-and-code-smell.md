# Compilation, Debugging and Code Smell

## Compile a source code into machine code (In C)

Compilation is the process of converting a source code into into machine code. That means into 0 and 1, that computers can understand. Here is what happens when you compile a source code in C :

1. Preprocessing

This consists in including all the necessary header files. In other words, all the external files that you included in your program in order to be able to use some parts of them, like some functions.

2. Compiling

This consists in taking the processed source code, ie, the source code with all including header files, and to convert it into assembly language.

3. Assembling

This consists in taking the assembly code and convert it into binary, also called machine code. This is the type of instructions that a computer can understand.

4. Linking

In the assembling step, all including header files are transformed into binary separately. That means they are not linking together. Linking step consists in taking all those chunks of binary codes and merge them together.

## DEBUGGING

Computer programmers usually call errors in there code : **Bugs**. **Debugging** is the art of *finding these errors and resolving them*. Here are three main ways that can facilitate you debugging a code:

1. Use the logs

This consists in printing some variables values at some points of your program in order to see what you exactly get. This will show you if the values are correct or not. This will give you some clues of where your program is breaking. Maybe the problem comes from a variable that does not have the right value.

For example :

- In `C`, you can log the values of your program by using the `printf` function
- In `JavaScript`, you can log the values of your program by using `console.log()` 

2. Use breakpoints

You can use breakpoints to control the execution of your program. By adding breakpoints, you can pause the execution of your program wherever you want. This will help you clearly see how your program is executed step by step and discover where something goes wrong.

If your code editor or IDE don't have the feature to set breakpoints to debug your code, you should consider using another one... Because this is one of the most important debugging techniques you should have in your developer's toolbox.

3. Talk out loud to yourself

You can talk out loud the execution of the code as the way it should normally work. It's like explaining to yourself the steps of the execution of the program while you verify if what you are saying is exactly what the code you write does. If somewhere what you say is not similar with the code that is written, that means there is a problem there.

## Code smell

Code smells are nothing but some pratices that can make your code unreadble, hard to maintain, difficult to evolve. In a nutshell, code smells are bad practices that make your code stinks.

### An Example of code smell

Let's say you have three lines of code that do a specific job. You need these lines of code in different places. So you copy and put them everywhere you need them. That practice is a code smell.

### WHY ?

If a day you realize that you were wrong about the logiq behind these three lines of code, you'll have to go in all the places where you copy them to make the same modifications. If it's a huge project, this can be really disturbing.
   
To avoid that code smell, it would be better to put these three lines of code in a function, and call this function anywhere you need it. If a day you need to change the logiq of these three lines of code, you'll only have to modify that function that handles your code.