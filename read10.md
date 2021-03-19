# Reading Notes 10 Course 201

__*Order of Execution*__

In order to find the source of an error, you need to understand the order of execution ( order in which scripts are processed)

- Javascript interpreter uses the concept of excution contexts ( one global, each script creates a new execution content)

- Global Context - Code that is in the script but not in the function

- Function Context- Code that is in the script and within a function

__*Variable Scope*__

- Global Scope - When a variable is declared outside of a function it can be used anywhere because it is global

- Function Scope - When a variable is declared inside of a function, it can only be used within the function

__*The Stack*__

Javascript interpreter processes one line of code at a time, and when it needs data from another function, it stacks the function on top of the current task

- Each time a new item is added to the stack it creates a new execution context

__*Execution Context & Hoisting*__

Each time a script enters a new execution context it goes through 2 phases:

1. Prepare - a new scope is created, and variables functions and arguments are created

2. Execute - It can assign values to variables, reference functions and run their codes, and execute statements

- Each execution context has its own variable object and can access its own variables, functions, parameters, and its parents variable object

## Errors

If a statement generates an error it throws an exception. Javascript then stops and looks for exception-handling code

- You can use a set of statements to handle the error
- These statements will stop when they find an error and handle it
- If there is no error handler, the scriot will stop running and give you an error object

__*Error Object*__
An error object will help you find where mistakes are (browsers have tools to help as well)

To deal with errors you need to do two things:

1. Debug the script to fix the errors(Track down source and fix it)

2. Handle errors "Gracefully" - Fixing an error that is beyond your control (requesting data from third party, etc.)
You can "gracefully" check if something works, and offer an alternative if it doesnt

You can use console.log() to see what a script returns

Other console methods include

- Console.info , console.warn, console.error

- To group multiple sets of related data you can use console.group() and console.groupEnd() at the end to indicate the end of a group

Console.table() lets you output a table showing ovjects and arrays containing other objects and arrays

Console.assert() can be used to check if a condition is met

Breakpoints - used to pause the execution of a script on any line (web console)

- This is helpful to read through code line by line to see where values change and where errors can occur

You can also indicate that a breakpoint be triggered only when a condition that you specify is met

You can create a breakpoint in your code using the debugger keyword

You can use try, catch, and finally in your code to see if your code will fail

Try - Will try to execute the code
catch (exception) - If there is an exception, run the code

Finally - will always get executed

If you know where an error may occur in your own script you can generate your own errors in code
> throw new Error('message')

[<== Back to Main Page](README.md)
