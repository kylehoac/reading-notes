# Reading notes 04

## Process and Design

__*Who is visiting your website and why?*__

When creating a new webpage, one of the first things you want to figure out what demographic the website is targeting. Target groups consist of Individuals, and Companies, and will change based on what type of service or information the website provides. Once you figure out who is visiting your website, you can then figure out why they would visit your website, and what their motive is behind visiting it.

__*Site map and Wireframing*__

- Before creating your website you're going to want to create a *site map* which is a diagram showing how the pages on your website will be grouped. This allows the visitor to easily navigate through the website and find the exact information they're looking for.
- Your *wireframe* is a simple sketch of what needs to go on each page of the website. It shows the hierarchy of information and how much space everything needs.

You will need to create a visual hierarchy, so that when visitors are skimming through your website, they can find valuable information quickly. This is often done by using size, color, and style

__*HTML Structure*__

HTML pages are created in text documents. It uses tags which are characters inside of angled brackets. They act as containers and tell you something about the information between them. Tags usually come in pairs (opening and closing tags) however in some cases they are self closing. The opening tag will denote the start of a piece of content, while the closing tag denotes the end. Opening Tags can carry attributes that tell you more about the tag, and require a name and a value.

__*About HTML5*__

HTML5 introduces a new set of elemetns that allow you to divide up the parts of a page. The names of the elements indicate the kind of content you will find in them.

*HTML5 examples

- header and footer (contain the stuff at the top and bottom of the page)
- nav (contains major navigational blocks)
- article (A container for any section of a page that could stand alone, such as an individual article, blog entry, comment, or blog post)
- aside ; has 2 means ddepending on whether or not its inside of an *article* element (When inside an article, it should contain information that is not essential to the article. When outside of the article element, it acts as a container for content thats related to the entire page such as links to other sections of the site, a list of recent posts, a search box, or recent tweets by the author)
- section (groups related content together, and will typically have their own headings)
- h group (Used to group together a set of headers)
- figure (used to group together any content that is referenced from the main flow of the article ex: images, videos, graphs, diagrams, code samples, text that supports main body of an article.)
- div (groups together related elements)

__*Extra Markup*__

- <!-- used for comments. this text will not appear on the html document-->
- ID Attributes (Every element can carry an id attribute. They are used to uniquely identify that element from other elements. In terms of CSS, you can use ID Attributes to uniquely design certain elements. In JavaScript, you can use ID Attributes to allow the script to work with certain elements)
- Class Attributes (Used to identify several elements as being different from other elements. Its value describes the class it will belong to)
*By default using these elements does not affect the presentation of an element unless their appearance is being altered by a CSS rule that indicates it should be displayed differently*

- Block elements ( Elements that will always appear to start a new line in the browser window)

- Inline elements (Elements that will always appear to continue on the same line as their neighboring elements)

- Span elements (Acts as an inline equivelent to div. Uses include 1.Containing a section of text where there is no other suitable element to differentiate it from other text, 2. Contain the number of inline text)
*The most common use of span is to control the appearance of the content of these elements using CSS*

- iframe (used to create a little window that has been cut into the page. The attributes used with it include, src(specifies url of page) height, and width)

[<== Back to Main Page](README.md)
