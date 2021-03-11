# Course 201 Reading Notes 4

__*Links*__

Links are a feature on the web that move you from one webpage to another enabling browsing. They can bring you from

- one website to another
- another page on the same site
- from one part of a webpage to another
- to new browser windows
- to start up your email and address a new email to someone

__*Writing Links*__

- Links are created using the a element followed by the href attribute

> < a href = " ">text< /a >

- When linking to pages on the same website you use relative urls

__*Directory Structure*__

- The root folder in a directory is considered the parent folder
- A folder made in the root folder is considered the child folder
- A folder made in the child folder is the child of that folder, and the grandchild of the root folder etc.

A root folder contains an index.html file which is the homepage for the entire site, and other folders

The sub directory also contains an index.html, other folders, etc.

__*Relative URL*__

- Relative URLs are a shorthand way to tell the browser where a page is that is on another page

- If all the files in your site are in one folder, you just use the file nap for that page. This makes it faster to write since you dont have to write the entire domain naim

> Ex: < a href="page.html">Reviews< /a >

__*Email Links*__

You use the mailto: attribute to create an < a > link that starts up the users email program to a specified email address

> mailto:

__*Opening links in new windows*__

To open a link in a new window you use the target attribute

> < a href="https:google.com: target=:_blank" >

__*Linking to the same page*__

To link to a different part of the same page, you can use an elements id value

> < a href="#bottom" > ... < /a >
----------------------------------------------------------------------------

## Layouts (CSS)

CSS treats every HTML element like its in its own box
The box will either be block or inline

__*Block and Inline elements*__

> Block elements include
>> < h1 >, < p >, < ul >, < li >
----------------------------------------------------------------------------
> Inline elements include
>> < img >, < b >, < i >

Block level elements start on a new line and act as the building blocks of a layout

- If one block level element sits inside another block level element then the outer block is the containing or parent element

__*Positioning schemes*__

Normal flow

- Every block level element appears on a new line

Relative Positioning

- Moves an element from its normal flow position, and shifts it towards the left, right, top, or bottom of a page

Absolute Positioning

- This positions the element in relation to its containing element

__*Box offset properties*__

Fixed positioning

- Elements with fixed positioning dont effect the position of the elements around them and dont move when you scroll up and down a page

Floating Elements

- Floating an element allows you to take that element out of normal flow.

Normal flow
> position:static

Relative Positioning
> position:relative

Absolute positioning
> position:absolute

Fixed positioning
> positioning:fixed

Overlapping elements
> z-index: 0;

Floating Elements
> float: left/right;

Clear float
> clear: left/right;
>> Parents of floated element w/ border:
>>> overflow: auto;
>>>> width:100%;

You can create multi column layouts with floats using

> width, reset, and margin

- You need to take into consideration that visitors will be viewing the webpage from different screen sizes, and resolutions
- Most web developers will create pages ariybd 960 - 1000 pixels wide since most users will be able to see that

__*Fixed width layouts*__

Fixed with layouts dont change sizes when the user increases or decreeases their screen

__*Liquid Layouts*__

Liquid layout designs will stretch and contract when the user increases or decreases screen size

__*Functions*__

Functions let you group a series of statements together to perform a specific task. If different parts of a script repear the same task, you can reuse the function instead of repeating the same set of statements

- Grouping together statements that are required to answer a question or perform a task helps organize code.

- The statements in a function are not always executed when a page loads, so they can also be used to store the steps needed to complete a task. The script can ask the function to perform all of the statements within it when they are required.

- In order to make a function perform a task you need to give it a name that resembles what type of task its performing. When you ask a function to perform said task, it is called calling a function.

- The steps that a function needs to perform to do a task are packaged in a code block ( a code block consists of one or more statements contained within curly braces)

- Pieces of information passed on to a function in order to perform a task are known as parameters

- When you write a function and expect it to give an answer, the response is known as a return value

__*Declaring a Function*__

- To create a function you give it a name and then write the statements needed to achieve its task within curly braces. (Known as Function Declaration)

__*Calling a Function*__

- In order to call a function, you would write the function name followed by parentheses

- If a function needs information to work, you indicate what it needs to know in parentheses after the function name. These are Parameters

Parameters vs Arguments

- While some people use the terms interchangably, however there are subtle differences. A parameter is used like a variables, whereas an argument calls for the actual value of said variables

[<== Back to Main Page](README.md)
