# Reading Notes 7 Course 201

__*Tables*__

Tables display information in a grid format

- Each block on the grid of a table is referred to as a table cell
- To create a table you use the < table > element followed by a < tr > element to indicate the start of a row. Inside each tr element, you will use a < td > element to create a cell in the table

> < table > < tr > < td > < /td > < /tr > < /table>

To have an entry stretch more than one column you use the colspan attribute

To have an entry stretch more than one row you use the rowspan attribute
 
Headings of a row should sit in the < thead > element, while the body should sit in < tbody > and the footer should sit in the < tfoot >

----------------------------------------------------------------------------------------

__*Creating an Object using Constructor Notation*__
You create an object using the "new" keyword, and the Object() constructor function
> var hotel = new Object();

You then add a property to it. This is done by writing the object followed by a period and the "key" (value)
> hotel.name = 'quay';

You can then use the same syntax to add functions
> hotel.checkAvailability = function() { return this.rooms - this.booked; }

How to change the value of an objects property
> hotel.name = 'park';

How to change the value of an objects property ( not including the methods inside)
> hotel.[ name ] = 'park';

To delete or leave a property cleared
> delete hotel.name
>> hotel.name = ' '

__*Creating many objects*__

- First create a template using a function that has the parameters and methods of all of the objects

> function Hotel(name,rooms,booked){this.name = name; this.rooms = rooms this.booked=booked;}

- Create different instances of the object using the new keyword (creates a new object)

> var quayHotel = new Hotel('quay', 40, 25);

To access properties you will use dot notation to "call" the property ( hotel.name )

The this keyword is commonly used in functions to refer to a property within the scope of its object or function

__*Arrays are Objects*__

- An array is a special type of object that shows its data as index numbers instead of property names
- You can combine arrays and objects to make more complex data structure. The array can store a series of objeccts and remember their order, while an object can also hold arrays

__*Built in Objects*__
Browsers come with built in objects that come in 3 compartments

1. Browser Object Model - Objects that represent the current browser window or tab

2. Document Object Model - Objects that create a representation of the current page

3. Global Javascript Objects - Objects that represent things that the javascript language needs to create a model of

__*Object Model*__
A group of objects, each rerpesenting related things from the real world.

[<== Back to Main Page](README.md)