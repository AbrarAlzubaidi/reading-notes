## objects:
it's like a box gathering a set of variables and functions.
- any variable inside the object called property, which tells you about the object.
- any function inside the object called method, which is a task dea/connect with the object to do something.
- how to declare objects: 
     - `let objectName {
       //block of properties and methods
     };`

- after each property and method to separate them use `,`
- to separate keys and its value use `:`
- to access something inside the object you can use 2 ways
     - `objectName.property or method name`
     - `objectName[property or method name]`


----------------------------------------------


## DOM "document object model"
**works** hoe the browser should create a model of an html page and how JS can access and update the contents of the page while it is in the browser window.

### DOM has 2 primary areas:
1. making a model at html page:

DOM determine the way in which the browser should structure this model using DOM tree.

2. accessing and changing the html page:

DOM determine methods and properties to access and update each object in this model.

***some programmers called DOM "application programming interface API"***

### DOM tree:
stored in the browser's memory. it has 4 types of nodes:

1. document node.
2. element node:each element present as a node. each node present an object with methods and properties.
3. attribute node: contains the attributes that inside the node.
4. text node: contains the text that inside the element.

### how to access DOM tree:
1. allocate the node that contains the elements you want to access.
2. use its text, child element and attributes to make changes or delete it or add some new nods.

### how to select individual element:
1. `getElementByID()`: use the value to select the element that has the ID attribute.
2. `querySelector()`: use CSS selectors and return the first matching element.

**notes**

- individual element deals with object:document.
- those methods return one value.

### how to select multiple elements:
1. `getElementByClassName()`: select all the elements which have the same name of class.
2. `getElementByTagName()`: selectall elements that have the same tag name.
3. `querySelectorAll()`: use CSS selectors to select all matching elements.

**note**

- ithose methods return more than one value stores in nodelist.

### to move from element to element:
1. `parentNode()`: select the parent of the current element.
2. `previousSibling()/nextSibling()`: select the previous or the nect sibling for the current element.
3. `firstChild()/lastChild()`: select the first or the last child for the current element.

**notes**:
- those methods called "traversing the DOM".
- `nodeValue`: it is a property which allows you to modify the content of the text node.
- to access just text connect: `textContent` property.
- to access text connect and child element: `innerHTML` property.
- `createElement()`/`createTextNode()`/`removeChild()`: to create a new node, add it, or remove it.
- `hasAttribute()`/`getAttribute()`/`setAttribute()`/`removeAttribute()`: to update or get attributes.


### nodelist: 
similar to arrays but not exactly the same. it has an index to store each node that return.

- nodelist it is from a datatype called collections refers to object family.
- some methods deal with nodelist:
     - length: to return number of elements inside the nodelist.
     - item(): return specific node from the nodelist by its index.

- if you want to apply the same instuctions for each node use **loops**.


### how to add element:
1. create the element: `createElement`
2. give it content: `createTextNode`
3. add it to the DOM: `appendChild()`


### how to delete element:
1. store it in a variable
2. store its parent in a variable
3. remove the element: `removeChild()`.


***resources:***

1. JavaScript and JQuery Interactive Front-End Web Development.
