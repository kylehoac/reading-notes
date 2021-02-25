# Reading notes 06

__*How do HTML CSS AND JS interact with eachother*__

 When using the three languanges together, each language forms a seperate layer with different purposes.

- Html - This is where the content of the page lives
- CSS - Enhances the Html page with styles, colors, backgrounds, borders, etc.)
- JS - Changes how the page behaves and adds interactivity.
You want to keep this page seperate from the rest, so that it is usable even when JS is turned off. You can reuse this code on several pages, making it easier to maintain and faster to load. It is written in plain text, similarly to Html, and CSS, so you do not need any new tools to write JS. JS files end in .js.

__*Progressive Enhancement*__

- When the 3 languages are layered on top of eachother, they form the basis of *progressive enhancement*. It is currently the most popular approach to building a website.

- In order to use JS with Html and CSS, you need to use the *script* element in Html followed by the src attribute.

- Generally the best place to put your scripts is right before the closing body tag.

- You can also add your javascript in the Html file between the opening and closing script tags, however it is better to put them in their own files

__*How to use Objects and Methods*__

Example line of JS

- document.write('Good Afternoon')

In this line of code, "document" is the object.

- The document object represents the entire web page. All web browsers implement this object and you can use it just by giving its name.
- The write () method allows new content to be written into the page where the *script* element sits.
- Programmers refer to this as calling a method of an object.
- Java script will run where it is found in the Html. When the browser comes across a *script* element it will stop and load the script, then check to see if it needs to do anything.

## Basic Javascript Instructions

__*Statements*__

A script is a series of instructions that a computer can follow *one by one*.

Each individual instruction is known as a *statement*.

- JS is case sensitive

__*Comments*__

- /**/ - for multi line comments
- // - for single line comments

__*Variables*__

- *var quantity*
- var or let for *variable keyword* followed by a variable name
- *quantity = 3*

- assign the variable name a value preceded by an operator

__*Data Types*__

- Numeric (0.75)
- String Data Type ('text')
- Boolean (T/F)

[<== Back to Main Page](README.md)
