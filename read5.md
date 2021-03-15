# Reading Notes 5 Course 201

__*Images*__

- When building a website it is generally a good idea to have all of your images in folder specifically for images

You add an image by using the img tag followed by the src attribute. You can give the image a description using the alt attribute and a title using the title attribute. You can also adjust the image height and width using the height and width attributes

> < img src = "imagelink" alt="description" title = "title" height = "" width = "" >

Generally you want to place your image after a paragraph, inside of the start of a paragraph, or in the middle of a paragraph

3 rules to follow when creating images

1. Save images in the right format (png,jpeg,gif)
2. Save images at the right size (The images you use should be saved as same width and height that you want them to appear on your website)
3. Measure the images in pixels

Vector Images - Images that are resolution independent. These images are usefull because you can increase the dimensions of an image without affecting the quality of it

__*Figure and Figure Caption*__

Figure and figure caption are elements used to contain images, and give them a caption.

__*Color*__

color - property that defines the color of the text (you can use rgb values or hexcodes)

background-color - property that defines the color of the background of an element. Since each element acts as if it is its own box, it will change the color of the box that the element is inside of

opacity - used to change the opacity of an element (visibility). You can also use this for colors as well

__*Text*__

__*Typeface Terminology*__

Serif - traditionally used font in print

sans-serif - straight edged letters, easier to read on screens

monospace - commonly used in code

Weight - Light, Medium, Bold, Black

Style - Normal, Italic, and Oblique (normal font at an angle)

Stretch - Condensed, Regular, extended

Typeface - When using typeface, you need to remember that the browser will only display it if its installed on the users computer

Specifying type face
< font family >

Size of Font
< font-size >

Font Face + src attribute ( downloads to the computer of the person browsing )
< @font-face >

NOTE : Different browsers support different formats for fonts. You will supply the font in various formats

__*Text transform UPPERCASE and lowercase*__

> < uppercase; to make text appear in uppercase >
> < lowercase; to make text appear in lowercase >

__*Strike and*__

> text-decoration: none,underline,overline,line-through,blink

__*Leading*__
leading is used to determine the amount of verticle space between text
> line-height; 1.4em;

__*Text Align*__

> text-align: left,right,center,justify

__*Verticle Alignment*__

This is generally used with inline elements

> verticle-align;

__*Indenting*__

Indents first line of a text
> text-indent;

__*Drop Shadow*__

> text-shadow

__*First letter or line*__

> :first-letter , or  :first-line

__*Styling Links*__

Makes link look either unclicked on or visited
> :link , :visited

__**Responding to users**__

Pseudo classes that allow the appearance of the element change when the user interacts with it
> :hover , :active , :focus

## Attribute Selectors

existence - Matches a specific attribute.
> [] - p [ class ] targets all p elements with the attribute class

equality - matches a specific attribute with a specific value
> [ = ] - p [ class = "dog" ] targets any p element with the class attribute, ,and called dog

space - matches a specific attribute whos value appears in a space separated list of words
> [ ~= ] - p [ class~=dog ] targets any p element with an attribute of class and whos value is a list of space seperated words, one of which being dog

prefix - matches a specific attribut whos value begins with a specific string
> [ ^= ] - p[ attr^"d" ] targets any p element with an attribute whos value begins with d

substring - matches a specific attribute whos value contains a specific substring
> [ *= ] - p[ attr*"do ] target any p element with an attribute whos value contains letters do

suffix - matches a specific attribute whos value ends in aspecific string
> [ $= ] - p[ attr$"g" ] targets any p element with an attribute whos value ends in g

[<== Back to Main Page](README.md)
