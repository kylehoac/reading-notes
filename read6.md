# Reading Notes 6 Course 201

__**Objects**__

- An object groups together a set of variables/functions to create a model of something from the real world.
- In an object variables become known as properties and functions become known as methods

Functions - Tell us about an object, for example the name of a hotel or its number of rooms
Methods - Represent tasks relating to the object. EX: Check how many rooms are available by subtracting the number of booked rooms from the number of total rooms

- Properties and methods havea a name and value. In an object the name is called a key, and an object cannot have two keys with the same
- The value of a property can be a string, number, boolean, array or another object
- The value of a method is a function

- An object is the content inside of curly braces after a variable name. You separate the key from its value with a colon and separate each property and method with a comma (except for after the last value)

To use a value, you use the this. keyword that indicates the property it is using EX: this.room (ROOM is the value of a property)

- To access property or methods, you use the name of the object, followed by a period, followed by the name of the property or method you want to access

- The period is a member object. The property on the right is a member of the object on the left

You can also access he properties by placing them in square brackets instead []. You would most commonly do this when

- The name of the property or method contains special characters (like a dash)
- The name of the property is a number (generally avoided)
- A variable is being used in place of the property

__*Document Object Model*__
When the browser loads a web page it created a model of the page called the DOM tree.

It consists of 4 main types of nodes

1. The Document Node - Represents the entire page
2. The Element Node - Contains the elements of the html page
3. The Attribute Node - Contains the attributes of the elements of the html page
4. The Text Node - Contains the text within the elements

To access and update the DOM tree you want to

1. Locate the node that you want to work with
2. Use its text content, child elements and attributes

To access a single element you could use:
>getElementById() which uses the value of an elements id (This will use the document object which looks for the element anywhere within the page)
>>querySelector() which uses a CSS selector and returns the first matching element

To select multiple elements:
>getElementsByClassName() selects elements that have a specific value for their class attribute
>>getElementsByTagName() selects elements that have a specified tag name
>>>querySelectorAll() uses CSS Selector to match all matching elements

To access a text node you use the:
>firstChild property and then use the text nodes only property:
>>and then use the text nodes only property: nodeValue

- Methods that find elements in a DOM tree are called DOM queries
- If a method can return more than one node it will return a Node list which is a collection of nodes ( each node had an index number similar to an array) (You can use the length property to tell how many items are in the nodelist, similar to arrays as well) ( You can use the item() or item[] method to return the index number of a node in a collection.)
- You want to keep in mind that you want to use the least amount of nodes you can so that your webpage can operate quicker

There are 2 types of Node lists:
live - will update at the same time the page is updated, and will reflect changes in the script
static - the nodelist will not reflect changes in the script when a page is updates

You can loop through a nodelist and apply the same statement to each of the objects inside of it. You do this by finding out ow many items are in the nodelist, and then setting a counter to loop through them. Each time the script is run it wil check that the counter is less than the number of objects in the list

To go through the DOM you use the 5 properties of:
>parentNode
>>previousSibling, and nextSibling
>>>firstChild,lastChild

Some browsers will treat whitespace as a text node. You bypass this problem by using jQuery which helps deal with issues like this

__*How to update element content*__
When an element contains a mix of text and child elements, you should work with the containing element instead of each individual node

When accessing a text node, you will most commonly use the property:
>nodeValue

When working with an element you will most commonly use the properties:
>innerHtml - gets text and markup
>>textContent or innerText - gets text only

- When updating the content of an element it will overwrite the existing content that it originally contained

__*Adding or Removing Html Content*__
There are 2 different ways to go about adding or removing content from a DOM tree:

1. innerHtml property - It is used to retrieve and replace a node. It will update the content with a new string(to delete use an empty string)
2. DOM Manipulation - Creating a new element and text nodes and attaching them to a dom tree, or removing them from the DOM tree. To create content with DOM manipulation, you create nodes one at a time and store it in a variable. To remove

Steps of DOM Manipulation:

- Create element using

> createElement()

- Give it content using

> createTextNode()

- Add it to the DOM

> appendChild()

To remove:

1. Store the element to be removed in a variable

2. Store the parent of that element in a variable (var containerEl = removeEl.parentNode (remove el is first variable defined to be removed))

3. remove the element from its containing element using removeChild() method

When using innerHtml, beware of users using XSS (or cross site scripting) to take other users personal information or accounts. The attacker can place malicious code into your website that can access the websites information.

To avoid this to want to validate input going into the server, and escape data coming form the server and database

You also want to avoid where user content goes such as in

- script tags
- html comments
- tag names
- attributes
- css values

You can change an elements attributes by selecting the element of the attribute you want to change, add a period, and then use one of the following methods to get,check,change, or remove the attribute:

- getAttribute()
- hasAttribute()
- setAttribute()
- removeAttribute()

The property of these methods are className and id which will find the classname or id of the attribute

[<== Back to Main Page](README.md)
