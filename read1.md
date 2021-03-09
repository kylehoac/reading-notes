# Reading Notes 1 Course 201

HTML

- Html is used to create and structure a webpage. You start by writing down the words you want to appear on the page, and then further structure them by adding tags and elements

CSS

- CSS is used to control the styling and layout of the webpage. There are a variety of properties you can use to make the webpage look more appealing.

----------------------------------------------------------------------------
People access websites through a software called a "web browser". When you ask a browser for a webpage, the request is sent to the web server that hosts the website. In order to find the location of the web server, your browser will first contact the DNS server. Some companies offer web hosting, and for a fee they will host our website.

Small websites are often written with Html and CSS, however bigger websites will use a CMS (content management system), blogging tools, or e-commerce software which often utilize a few more technologies.

----------------------------------------------------------------------------

## General Structure of Html

html elements will be contained inside brackets called tags (<>) Here are the most common elements:

- DOCTYPE html
- html (contains the head and body)
- head
- body

Each element has an opening and closing tag (closing tags will have a / before the element name). Each element also tells the browser what to do with the information between the tags. Furthermore some tags are self closing, and some tags contain additional "attributes". Attributes contain more information about the contents of an element.

----------------------------------------------------------------------------

Extra Markup

- <!-- used for comments. this text will not appear on the html document
- ID Attributes (Every element can carry an id attribute. They are used to uniquely identify that element from other elements. In terms of CSS, you can use ID Attributes to uniquely design certain elements. In JavaScript, you can use ID Attributes to allow the script to work with certain elements)
- Class Attributes (Used to identify several elements as being different from other elements. Its value describes the class it will belong to)
*By default using these elements does not affect the presentation of an element unless their appearance is being altered by a CSS rule that indicates it should be displayed differently*

- Block elements ( Elements that will always appear to start a new line in the browser window)

- Inline elements (Elements that will always appear to continue on the same line as their neighboring elements)

- Span elements (Acts as an inline equivelent to div. Uses include 1.Containing a section of text where there is no other suitable element to differentiate it from other text, 2. Contain the number of inline text)
*The most common use of span is to control the appearance of the content of these elements using CSS*

- iframe (used to create a little window that has been cut into the page. The attributes used with it include, src(specifies url of page) height, and width)

----------------------------------------------------------------------------

### HTML 5 Layout

- header and footer are used to contain the main header and footer at the top and bottom of the page respectively

- nav is used to contain the navigational block used to access different parts of the webpage

- article acts as a container for any information that can stand alone such as an article, blog entry, a comment or post, or any other individual piece of content

- aside has two purposed depending on whether its inside or outside of an article element. If it is inside, it should contain information thats related to the article but not essential to its overall meaning. If it is outside of the article element, then it acts as a contaner for content thats related to the page as a whole (could contain links to other parts of the site, a search box, etc.)

- section is used to group related content together (ex: latest news, related pictures, products, etc.)

- hgroup is used to group together h1 - h6 tags, and treats them as a single heading (ex: title and subtitle)

- figure can contain any content thats referenced from the main flow of the article. It should always contain a figcaption element which provides a text description for the content. (ex: pictures, videos, graphs, etc.)

- div is used to group together many related objects. While its being used less, it should still be used if no other elements are suitable to group together your content

- You can turn a block level element, and all of the contents within it into a link using the a tag followed by the href element.

----------------------------------------------------------------------------

#### Process and Design

- When creating a webpage, you want to cater it towards your target audience. To do this you need to consider who the site is for, why they visit your website, what they are trying to achieve by visiting the website, what information/products do they need, and how often they will be visiting the site.

- To organize this information, web developers will use site maps, to organize the information into seperate sections. After this they will use wireframes, to show where that informaton needs to go ,how the information is presented from a hierarchical standpoint, and how much space everything will take up.

----------------------------------------------------------------------------

##### The ABC of programming

A - What is a script and how do I create one

- A script is a series of instructions that the computer follows to achieve a certain goal

- Each time a script runs, it mght only use a subset of instructions based on whether or not certain conditions were met.

- To help write a script, break the goal down into a series of tasks and then work out each step needed to complete the task

B - How do computers fit in with the world around them

- The computer will create models of the world using data

- Within a script, events can trgger methods, and methods can retrieve or update an objects properties

- In a script, the code basically says "When this event happens, run the code"

C - How do I write a script for a webpage

When using the three languanges together, each language forms a seperate layer with different purposes.

- Html - This is where the content of the page lives
- CSS - Enhances the Html page with styles, colors, backgrounds, borders, etc.)
- JS - Changes how the page behaves and adds interactivity.
You want to keep this page seperate from the rest, so that it is usable even when JS is turned off. You can reuse this code on several pages, making it easier to maintain and faster to load. It is written in plain text, similarly to Html, and CSS, so you do not need any new tools to write JS. JS files end in .js.

Progressive Enhancement

- When the 3 languages are layered on top of eachother, they form the basis of *progressive enhancement*. It is currently the most popular approach to building a website.

- In order to use JS with Html and CSS, you need to use the *script* element in Html followed by the src attribute.

- Generally the best place to put your scripts is right before the closing body tag.

- You can also add your javascript in the Html file between the opening and closing script tags, however it is better to put them in their own files so that they dont interfere with eachother.

[<== Back to Main Page](README.md)
