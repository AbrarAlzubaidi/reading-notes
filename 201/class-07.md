## tables in html:
table is a type of formatting style that represents information.

**table tags**:

1. `<table>`: to create the table.
2. `<tr>`: to initialize the start of each row.
3. `<td>`: to indicate the cell of rows.(contains the content.)  
4. `<th>`: to represent the header for column or row.
5. `<thead>`: to contain the header of long table.
6. `<tbody>`: to contain the body of long table.
7. `<tfoot>`: to contain the footer of long table.

- **notes**:
    - even the cell is empty you should write `<td>` tag. if you not the table will become a mess.
    - colspan attribute: to combine the adjacent cells as one cell.
    - rowspan attribute: to combine the rows that above each other to one row.
    - you control table size by: `width`, `cellpadding`(add spaces inside the cell) and `cellspaning`(add spaces between cells).
    - you can style it by adding `borders`,`background` and `text color`.


---------------------------------------------------


## Objects:
there is 2 ways to create an object:

1.literal notation:

      
       let objectName = {

        // block of code

       }


2. object constructor notation:


       let objectName = new constructorFunctionName();





*** from here till the end describe how to deal with the way 2***



- constructor: it is a function contains the initialization of properties.
- to add properties and methods to the object you should use *dot notation*.
- to update property just use dot notation to reach it and re-assign it to another value.
- to delete it, use delete keyword `delete objectName.property;`
- the name of constructor function shouldbe capital letter, to specialize it between the other functions.


### to create many object:
use the constructor function as a templete to the all objects which have the same properties.

      function constructorName (properties){

        // block of code.
      }
   

- `this` keyword: it means this property modify it, assign it or delete it. we use it inside the object body to reach propertiesand methods.


### why we call arrays are type of object?
because it hold a related values and its key is the index.

- arrays can store objects: `array[index].property`
- objects can hold arrays: `objectName.array[index]`


### build-in functions:

1. browser object model: contains objects that represent the current browser window. ex: `document`.
2. DOM: use Objects to create elements of the current page. ex: `getElementByID`
3. global JS objects: these in JS. ex: `string,number,...`


- note: 
   - string, number, boolean, undefined, null: are a simple datatype. *BUT* object is a complex datatype



***resources:***

1. JavaScript and JQuery Interactive Front-End Web Development.
2. HTML  CSS Design and Build Websites by Jon Duckett.