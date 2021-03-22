# Reading Notes 9 Course 201

## Form Conrols

__*Text,  Choices, Submitting, Uploading*__

Text Input
> For a single line of text

Password Input
> A single line of text that hides the characters

Text Area
> For longer areas of text such as messages and comments

Radio Buttons
> For making one choice

Checkboxes
> For making more than one choice

Drop down boxes
> Picking one option from a list

Submit Button
> Regular submit button

Image Button
> Lets you use an image

- The user fills in form information and presses the button to submit the information to the server

- Submitted information will come back in a name and value pair

__*Form Structure*__

Form conrols live inside of a < form > element. The element should always carry the action attribute

> < form action = "" method = "" >

To give the user more control over how your button appears you use < button >

- Each form should have its own < label > element. This makes the form accessibl to vision impaired users

- You can group related forms together using

> < fieldset > with < legend > inside of it (Description of group function)

Many forms need information such as dates, email addresses, and URLS. The element used to control this is
> < input > followed by the type attribute

The type attribute can be:
> "date" , "email", "url", or "search"

You can also use the placeholder attribute which will be the default text in the textbox before it is typed into.

## Events in JS

There are many different types of events that can trigger a function in Javascript

When an event has occurred it has been fired or raised

UI Events
> load, unload, error, resize, scrll

Keyboard Events
> keydown, keyup, keypress

Mouse Events
> click, dblclick, mousedown,mouseup, mousemove, mouseover, mouseout

Focus Events (when an element gains or loses focus)
> focus , blur

Form Events
> input, change, submit, reset, cut, copy, paste, select

Mutation Events (events that change the dom structure by script)
> DOMSubtreeModified, DOMNodeInserted, DOMNodeRemoved, DOMNodeInsertedIntoDocument, DomNodeRemovedFromDocument

__*Events are triggered by*__

1. Selecting Element

2. Specifying the event

3. Calling the code

Three ways to bind an event to an element :

- html event handlers ( old and bad practice )

- Traditional DOM Event Handelers (one event triggers one function)

> element.onevent = functionName;

- DOM Lv 2 event Listeners (one event may trigger multiple functions)

> element.addEventListener('event', functionName , boolean);

__*Using Parameters With Event handlers/listeners*__

In event handler you want to wait until an event triggers to call the function. If you need to pass an argument into a function, then you would wrap the function in an anonymous function
> el.addEventListener('blur', function(){checkUsername(5); false})

__*Event Flow*__

Html elements nest inside other elements, so if you hover or click on an element, you are also hovering or clicking on its parent elements.

- Event bubbling - The event starts at the most specific node and flows outwars to the least specific one (most widely used)
- Event Capturing - The event starts at the least specific node and flows inward to the most specific one

The flow of events usually only matters if you have an event handler on an element

The true or false you write in the event handlers and listeners are event capturing and event bubbling respectively (hence why false is often used)

__*Event Objects*__
When an event occurs the event object provides information about the event

It will tell you:

- Which element the event happened on,
- Which key was pressed for a keypress event,
- What part of the viewport the user clicked on

When an event object is passed into a function it is often given the parameter name e

__*Event Delegation*__
If users interact with a lot of different elements, they will use up a lot of memory when you need to add an event for every single element

- You an attach an event listener to a containing element which will target the property that the event is on using the target property
- By attaching an event listener to a containing element, you are only responding to one element, which delegates the job of the event listener to the parent

__*Changing Default Behavior*__

preventDefault()
> Prevents the default behavior of an elemnt when an event is triggered

stopPropagation()
> Stops an event from bubbling up to its ancestor once an event has been handled (useful if there are other event handlers responding to the same element)

return false;
> prevents default behavior, and bubbling to the parent (both)

To tell which element an event occured on you use the events "target" property

__*Different types of events*__

W3C DOM Events - Dom events are managed by W3C ( HTML,CSS XML ) (Most events are W3C Events)

HTML5 Events - Events that browsers can support that are used with HTML

BOM Events - Browser events (generally used with touchsceen devices)

__*Focus and Blur Events*__
If you interact with an Html element it gains focus. These events are triggered when an element either gains or loses focus (Focus = gain Blur = lose)

[<== Back to Main Page](README.md)
