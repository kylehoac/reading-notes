# Course 201 Reading Notes 3

__*Lists*__

Html offers 3 types of lists

- Ordered lists - each item in ordered lists are numbered

> Created with < ol >
>> each item in the list is placed between < li > tags

- Unordered lists - each item in unordered lists are bulleted

> Created using < ul >
>> each item in the list is placed between < li > as well

- Definition lists - made up of a set of terms and their definitions

> Created using < dl > followed by < dt > whcih contains the term and < dd > which contains the definition

__*Nested Lists*__

Nested lists are a second set of lists inside of another. You can do this by starting another list inside of an < li > element

__*Boxes*__

You can set up properties that effect a boxes dimensions, borders, margins, padding, and visibility

- A boxed dimensions is edited using *width* and *height*

> div {
    height: 300px;
    width: 300px;
}

- Furthermore you can limit the width and height of a box by using min-width, max-width, and min-height, and max-height

__*Overflow*__

Overflow property tells the browser what to do if the contents of the box are bigger than the box itself

- hidden - this property will hide all of the extra contents
- scroll - this property will add a scrollbar to the box to see the missing content

> div {
    overflow: hidden;
}
>> div {
    overflow: scroll;
}

__*Border, Margin, and Padding*__

Border - Seperates the edge of one box from another
Margin - Sits outside of the edge of a border, and can create a gap between the borders of two adjacent boxes
Padding - The spae between the border of a box and the contents within it

- Padding and margin are used to add space between the items on a page

__*Centering Content*__

> text - align: center;

__*Change Inline/Block*__

> display: inline / block

inline - Will change block elements to act like inline
block - Will change inline elements to act like block elements
none - hide contents (still viewable in view source)

__*Hiding Boxes*__

> visibility: hidden / visible

Hidden - Hides an element
Visible - Shows the element

__*Border Images*__

Applies an image to the border of a box. To do this you need the:

1. URL of the image
2. Where to slice the image
3. What to do with the straight edges

- Possible values include stretch (stretches image), repeat (repeats image), and round (similar to repeat but if the tiles dont exactly fit, they will be scaled so that they will)

__*Box Shadows*__

> box-shadow

You can adjust the horizontal, and verticle offset, as well as the blur distance and spread of a shadow

__*Rounded Corners*__

> border-radius

The values are used to indicate the size of the radius in pixels

- You can create elliptical shapes by specifying different distances for the horizontal and vertical parts of the rounded corners.
__*Arrays*__

An array is a special type of variable that can store a list of values.

- You would use an array when you are working on a list of values that are related to eachother
- They are helpful when you dont know how many items a list contains

> var colors;
>>colors = [ ' white ' , ' black ' , ' custom ' ]

- Values in arrays are treated like a numbered list starting from 0 (white would be 0, black 1 , and custom 2)

- To access items in an array you would specify the array name with the item number inside of brackets

- Here itemThree is declared

> var itemThree;
>> itemThree = colors[ 2 ]

- Every array has a property called length that holds the number of items in an array

> var numColors;
>> numColors = colors.length;

__*If.. Else Statements*__

The if else statement checks  condition, and if it resolves to true, than the first line of code will be executed. Otherwise the second block will be executed

> Ex: If (score >= 50) {
    pass();
}
else{
    fail();
}

- If else statements let you set two sets of code

1. one for if the condition evalauates to true
2. one for if the condition evaluates to false

__*Switch Statements*__

Switch statements start with a variable called the switch (value)

> switch (variable) { case 'one' : title = 'level one' break;} case 'two' ... case 'three'... default

- Each case acts as a variable, and will break if conditions are met. default will run if none of the cases conditions are met

__*Type Coercion & Weak Typing*__

Type Coercion - JS will convert a numbers data type to complete an operation ex ('1'>0) will turn '1' to 1

- Javascript used weak typing because the data type of a value can change

- other languages whos data types have to be strictly specified, use strong typing

__*Truthy and Falsy Values*__

- Truthy values - True
- Falsy values - False

__*Short Circuit Values*__

- Logical operators are processed left to right and will short circuit as soon as they come across a result, and return the value that stopped the processing

__*Loops and Loop counters*__

- Loop checks a condition. If it returns true, a code block will run. It will then check a condition again, and if it still returns true, then the code block will run again. This will continue looping until the condition returns false.

Types of loops include:

- *for* - Used for if you need to run a code a specific number of times. The condition is usually a counter which is used to tell how many times to run a loop Ex: for (var i = 0; i < 10; i++>). This code would write 0123456789 on the page with a document.write(i) code following it.

- *while* - Used for if you dont know how many times the code should run. The code will loop for as long as the condition is true.

- *do while* - Similar to the *while* loop, however will always run statements inside of curly braces at least once, even if the condition is false.

A for loop uses a counter as a condition. The condition is made of the following 3 statements:

- initialization - Create a variable and set it to 0. The variable is commonly called *i*, or *index* and acts as a counter. ( var i = 0;)

- condition - The loop should continue to run until the counter reaches a certain number. (i < 10)

- update - every time the loop has run the statements in the curly braces, it adds one to the counter (i++) (can also use -- to count down)

[<== Back to Main Page](README.md)
