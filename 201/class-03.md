## list types:

1. order list:use numbers at the beginning. to make order list use:

- `<ol>` tag: to craete it.
- `<li>` to put the content inside it.

2. unordered list: to make it:

- `<ul>` tag: to create it.
- `<li>` to put the content inside it.

3. definition list: used if you want to define something and you dont want to use `<p>` tag and any other tag.contains 3 tags:

- `<dl>` to create it.
- `<dt>` to contain which word/term you want to define it.
- `<dd>` the definition word.



**Nested list:**

alist inside a list. you can use any tags from above.


   ex: 

      `<ul>`

     `<li>`name1`</li>`

     `<li>`name2

    `<ul>`

    `<li>`first name`</li>`

    `<li>`last name`</li>`

    `</ul>`

    `</li>`

    `</ul>`



## boxes:

box is a sized area big enough to hold its content.**Css** treats each element as if it has its own box.

- to control box's dimensions you can use width and height properties.
- to limiting them use 
   - min-width: contains minimum size of box.
   - max-width: to contains maximum size of box.
   - min-height: same as min-width.
   - max-height: same as max-width.

   **these usage when the browser window is narrow or wide. to make the box flexible**



## overflow:

tells the browser what should do if the box contains content larger than its area. its values:
- hidden: hide any extra content.
- scroll: add scrollbar.


## borders:

it is the edge of one box. its like the surrounding line surround it.
- you can control the whole border width by: `border-width` 
- you can control one side of the border by : 
     - `border-top-width`
     - `border-right-width`
     - `border-left-width`
     - `border-bottom-width`


- you can style it by: `border-style` and it has 8 styles.
- you can change color the whole border by: `border-color`
- to change seperated sides by:
    - `border-top-color`
    - `border-right-color`
    - `border-left-color`
    - `border-bottom-color`


## padding:

space between the border and the content.

- you can change the whole padding by: `padding`
- to change seperated :
    - `padding-top`
    - `padding-right`
    - `padding-left`
    - `padding-bottom`



## margin:

space between the child element and its parent element OR the space between elements in the same parent.

- you can change the whole margin by: `margin`
- to change seperated :
    - `margin-top`
    - `margin-right`
    - `margin-left`
    - `margin-bottom`


**the benifit of padding and margin is to add some clear spaces between elements to make them stylish.**



## some important properties:

- `text-align: center`: to center the text.
- `display`: has 4 values:
    - inline: to change block element into inline element.
    - block: to change inline element into block element.
    - inline-block: to change block element into inline element.but still has its features.
    - none: hide the element in the page.

- `visibility`: to hide boxes. 2 values:
    - hidden: make it invisible.
    - visible: make it seen.



## some properties in CSS3:

- `border-image`: applay an img to border.requires:
    - URL for the img
    - where to slice the img
    - what to do with the straight edge.

- `box-shadow`: to add shadows to boxes.
- `border-radius`: to round the corner of the box also to make elliptical shapes.


---------------------------------------------------------


## JS:

- variables: it is like a space that stores data.its value could change or still as it.

- Arrays:it's a special type from variables can store more than one value.
- switch allow you to compair a value against posiible outputs.
- JS weak typing that mean you dont have to specify more about datatype.
- JS is a type coercion: can convert datatypeto complete a operation.to reduce it we can use `===`,`!==`


## falsy values: 

means if this statement is false explicity or un-explicity.



## truthy value:

means if this statement is true explicity or un-explicity.


**note:** logical operators called short circuit because they stop when they get the result. regardless its value.


## loops:

generally, to re-do somthing again for number of times.



### loop types:

1. for loop:usually we use it if we know number of iterations and for print array's elements.

ex: 

    for(initialization;condition;update)
    {
      // do s.th
    }


2. while loop:usually we use it if we dont know number of iterations (number to repeat the code).

ex: 

    initialization;
    while(condition)
    {
      // do s.th
      update;
    }


3. do-while loop: to do some code firstly then check the condition

ex: 
 

    initialization;
    do{
      // do s.th
      update;
    }
    while(condition)


## key loop:

1. break: to stop execution and jump to the next statement.
2. continue: to continue execution.


***resources:***

1. HTML  CSS Design and Build Websites by Jon Duckett.
2. JavaScript and JQuery Interactive Front-End Web Development.