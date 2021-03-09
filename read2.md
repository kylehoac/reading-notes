# Course 201 Reading Notes 2

## Structural / Semantic Markup

- **Structural Markup** - Elements used to create headings and paragraphs
- **Semantic Markups** - Elements that provide extra information such as emphasis in a sentence, something in quotes (and who quoted it), acronyms etc.

----------------------------------------------------------------------------
__*Structural Markup*__

__*Headings*__

> Can go from
>> < h1 - h6 >

- Text inside will be headings
- h1 is used for main headings
- h2 - h6 are used as subheadings

__*Paragraphs*__

> < p >

__*Bold & Italic*__

 Bold
> < b >

Italic
> < i >

__*Superscript & Subscript*__

Superscript
> < sup >

Subscript
> < sub >

__*White Space*__

Known as *white space collapsing* if two or more spaces appear together they show up as only one space. This can creat space in the code, and make it easier to read while displaying normally. If it comes across a break it will show as one space as well.

__*Line Breaks & Horizontal Rules*__

You can create a line break in the middle of a paragraph using
> < br / >

You can create a horizontal rule using (horizontal line breaking text)
> < hr / >

__*Semantic Markup*__

strong - Contents are bold
> < strong >

em - contents are italic
> < em >

__*Quotations*__

blockquote - used for long quotes that could take up a paragraph
> < blockquote >

q - used for shoter quotes that are within paragraphs. (generally avoided as internet explorer doesnt support it)

__*abbr*__

abbr - used for abbreviations and acronyms. A title attribute is used on the opening tag
> < abbr title = "" > < /abbr >

__*Citations & Definitions*__

cite - used when referencing a piece of work to indicate where the citation is coming from
> < cite >

dfn - used for when you explain new terminology or concept.
> < dfn >

__*Author Details*__

address - used to contain the authors contact information and details, such as email, and address

__*Changes to content*__

ins - used to show content that was inserted into a document (underlined)
> < ins >

del - used to show content that was taken out of a document (crossed out)
> < del >

s - similar to del, but used to indicate something that isnt accurate anymore (crossed out)
> < s >
----------------------------------------------------------------------------

__*CSS Introduction*__
CSS stands for Cascading style sheets. It is a programming language used to give color, animation, and style to html sheets.

- The best way to imagine how CSS works is to imagine an invisible box around every Html element
- CSS creates rules that changes the way the content in Html elements are presented
- CSS associates rules with HTML elements. CSS rules contain two parts: a *selector* and a *declaration
- Selectors indicate which element the rule applies to. You can apply the same rule to more than one element by seperating the element names with commas.
- Declarations indicate how elements referred to in the selector should be styled. Declarations are split into two parts, (property, and value) that are seperated by a colon ;
- You can use CSS rules in an html document if you surround them in a *style* element (inline styling)

__*External CSS*__
 link - is used to tell the browser where the CSS document used to style the page is located
> < link attribute >

It is followed by the attributes href, type, or rel

href - specifies path to CSS file (file name)

type - specifies type of document being linked ( usually "txt/css" )

rel - indicates the relationship between the html page and the file that its being linked to ( usually "stylesheet")

__*Internal CSS*__

style - You would use the style tag within the element that you want the CSS to change. Inside of the style element you can use CSS syntax

| Selector        |  Use          | Ex  |
| ------------- |:-------------:| -----:|
| universal      | applies to all elements on the age | * {} |
| type     | specific element names      |   h1,h2,h3 {} |
| class | specifies specific class elements |   .note {} or p.note {} "paragraph with note class"|
| id |   matches element whose id attribute matches the one specified after #         | #introduction {}
| child | matches the child element of another   |  li>a {} (taregets a elements that are children of li element)
| descendant |       matches element that is the decendent of another element   |   p a {} (targets a elements sitting inside of p elements)
| adjacent sibling | matches element that is a sibling of another   | h1+p {}
| general sibling  |    matches element that is a sibling of another regardless of it being directly preceding or not     |   h1~p {}

__*How CSS Rules Cascade*__
If there are two or more rules applied to the same element, the last rule will override the first rule. If one rule is more specific than another rule, than the more specific rule will over ride the more general one. (a type selector will show over a universal selecor)

__*Inheritance*__
You can force values of child elements to inherit the value of the parent elements properties by using inherit for a value. Certain properties from a parent element such as font, or colors will automatically be inherited by their child elements, whereas background wont.

----------------------------------------------------------------------------

__*Basic Javascript instructions*__

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

__*Using a Variable to store numbers and strings*__

- When using a variable to store a number make sure not to put it in quotation marks, or it will be considered a string
- If you want to store a string, than write the variable name inside of quotation marks
-You can use quotes inside of a string by either putting single inside of double, or double inside of single quotes

__*Changing the value of a variable*__

- You can change the value of a variable later on within the same script, if a set of statements leads to it, or if you put the variable name and an equals sign later on in the script.

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

__*Comparison Operators : Evaluating Conditions*__

- Comparison operators can evaluate a situation by comparing one value in the script to what you expect it might be. The result will be boolean

*==* - Is equal to
*!=* - Is not equal to
*===* - Strict equal to (Compares two values to check that the data type and value are the same)
*!==* - Strict not equal to (Compares two values to check that the data type and value are *not* the same)
*>* - Checks if the number on the left is greater than the number on the right
*<* - Checks if the number on the left is less than the number on the right
*>=* - Checks if the number on the left is greater than or equal to the number on the right
*<=* - Checks if the number on the left is less than or equal to the number on the right

__*Logical Operators*__

- Logical operators allows you to compare the results of more than one comparison operator

*&&* - Tests more than one condition. If both expressions evaluate to true then the expression will return true. If one of the expressions evaluates to false, then the expression will return false.
*||* - Tests at least one condition. If either expression evaluates to true, than the expression will be true, if both expressions evaluate to false, then the expression will be false
*!* - This operator takes a single boolean value and inverts it. EX: !(2 < 1). This expression was false without the !, however with it, it returns as true

- Logical expressions are evaluates left to right. If the first condition can provide information to get the answer, then there is no need to evaluate the second expression

__*If and If Else Statements*__

An if statement is used to check a conditio (true or false)

- If the statement resolves to true, than any subsequent code in the block will be executed. If the statement resolves to false, then the statements in that code block will not run

- an if else statement checks a condition, and if it resolves to true, than the first block of code is execute. Otherwise the second block will be executed instead

[<== Back to Main Page](README.md)
