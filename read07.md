# Reading Notes 07

__*JavaScript*__

- Javascript can be used in browsers to make websites more interactive, interesting, and user friendly
- Javascript uses jQuery to make writing js easier
- Javascript can also be used to add elements, attributes, and text to a page (or remove them)
- You specify a set of steps for the browser to follow, which allows it to change or access certain contents of a page. You can also specify that a script could be run when a specific event has occurred, or if a specific event has been triggered by the user or browser
- To change the content of an Html page while it is loaded in a browser, the browser must be able to
- Access the content of the page
- Modify the content of the page
- Program rules or instructions the browser can follow
- React to events triggered by the user or browser

*What are scripts?*

- A series of instructions that a computer can follow to achieve a goal
- A browser will use diferent parts of the script depending on how the user interacts with the page
- Scripts will run different sections of code in response to the situation around them
- To write a script you need to state your goal, and then list the tasks needed to achieve it
Steps to creating a script:

1. Define a goal
2. Design the script
3. Code each step

You will need to define tasks, and then code in the series of steps needed to complete said task

__*Expressions and Operators*__

Expressions result in a single value. There are 2 types of expressions

1. Expressions that assign a value to a variable

(var color  = "beige")

2.Expressions that use 2 or more values to return a single value

(var area = 3 * 2) ( alternatively you could also combine 2 strings)

Expressions rely on things called operators; they allow programmers to create a single value from one of more values

Arithmetic Operators include:

    + - / * ++ -- %

- Arithmetic Operators will follow PEMDAS
- Arithmetic Operators are used to calculate the value of two or more costs

String Operators include:
    +
String operators will combine 2 strings using the + operator
ex: var firstName = 'kyle';
    var lastName = 'hoac';
    var fullName = firstname + lastname; RESULTING IN = kyle hoac

- When you place quotes around a number, it is a string ex: '2' is a string not a number. You can combine numbers and strings together doing this

ex: var cost1 = '7';
    var cost2 = 'nine';
    var total = cost1 + cost 2 RESULTING IN '7nine'

__*Functions*__

Functions let you group a series of statements together to perform a specific task. If different parts of a script repear the same task, you can reuse the function instead of repeating the same set of statements

- Grouping together statements that are required to answer a question or perform a task helps organize code.

- The statements in a function are not always executed when a page loads, so they can also be used to store the steps needed to complete a task. The script can ask the function to perform all of the statements within it when they are required.

- In order to make a function perform a task you need to give it a name that resembles what type of task its performing. When you ask a function to perform said task, it is called calling a function.

- The steps that a function needs to perform to do a task are packaged in a code block ( a code block consists of one or more statements contained within curly braces)

- Pieces of information passed on to a function in order to perform a task are known as parameters

- When you write a function and expect it to give an answer, the response is known as a return value.

__*Declaring a Function*__

- To create a function you give it a name and then write the statements needed to achieve its task within curly braces. (Known as Function Declaration)

__*Calling a Function*__

- In order to call a function, you would write the function name followed by parentheses

- If a function needs information to work, you indicate what it needs to know in parentheses after the function name. These are Parameters

Parameters vs Arguments

- While some people use the terms interchangably, however there are subtle differences. A parameter is used like a variables, whereas an argument calls for the actual value of said variables

[<== Back to Main Page](README.md)
