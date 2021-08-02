## links:
used for making user move from page to another page.

### how to write links:

`<a href="URL">page_name</a>`

### to make a list of links:

by define `<ul>` tag, inside of it `<li>` tag, inside of it `<a>` tag. so it will show like:

`<ul>`

`<li><a URL">`
`name1</a></li>`

`<li><a URL">`
`name2</a></li>`

`</ul>`

**notes:** 
- make each section on the page in different directory/folder to make it not too long and easy at error detiction process.
- each directory has its own path.

### file's path:
there is 5 way to type the URL depend on where is the html file:

1. same folder: if the file is not in any folder so it reacte like a folder. `**URL:** "filename.html" `
2. child folder: if the file inside a folder. **URL:** `"foldername/filename.html"`
3. grand folder: if the file inside a folder that inside a folder. **URL:** `"foldername1/foldername2/filename.html"`
4. parent folder: to indicate the folder above the current one. **URL:** `"../filename.html"`
5. grang parent: to indicate that you want to go up two folders. **URL:** `"../../filename.html"`


### what about emails can they defined like the normal links?
no, the browser will not recognize it as an email. it will recognize it as a normal email. to fix that use: `mailto` (to tell the browser it is an email link.) inside the URL.

ex:

`mailto:username@example.org`

### previous ways to add link open it in the same tab. what if we want it to open in different tab?
by using `target` attribute.The value: ` _blank`

ex:

 `<a href="http://www.google.com" target="_blank">`

### to link a specific element/part in the page + in different page.you need to:
identify the points in the page that the link will go to. by the id attribute. the value of the href attribute starts with the #, then the name of the id attribute of the element you want to link it.   `<a href="#id1">name1</a>`



------------------------------
## layout:
CSS can control the position of the elements using many of attributes, such as:

1. position: its value 
     - static 
     - Relative
     - absolute

2. text-align: to position the text
3. padding.
4. margin
5. float: its value:
    - left
    - right
    - none
    - inherit
6. display



----------------------------------



# Functions

**Functions** is a block of code/instruction that make you do something. we use it to use the block of code more than one time and to organize our programming code to make it more readable.

#### so, what is the type of functions in JavaScript:
1. function declaration

    **syntax:**


     function function_name (){

       //block of code
       
     }
- you can call it by its name like: 

     function_name();



2. function expresiion

    **syntax:**


     var function_name = function(){

       //block of code
       
     }

3. var area = (function()
var wi dth = 3;
var height = 2;
return widt h * height;
}());

this function are not given
a name. Instead, they are executed once as the
interpreter comes across them.


 - also you can call it like previous one.by its name.

 ------------------------------------------------
 
 
 ### those two types can be classified about have/have not parametres to:
 1. function with parameter/s:

 it means you have to pass to this function some arguments
     **syntax:**


     function function_name (parameter1,parameter2,...){

       //block of code
      
     }

  - the calling will be :

  function_name(argument1,argument2,...)

 2. function without parameter:

    **syntax:**


     function function_name (){

       //block of code
       
     }
  - it like the original function and the calling is the same of original function.

### those two types also can be classified about return value or not:

1. return function:


    function function_name (){

       //block of code
       // here you have to return the value of something 

       return x;

     }

 2. non-return function:


     function function_name (){

       //block of code
       // there is no need to return the value but to see/show your result you should type 
       console.log(value)  // to show it in console

       OR 

       document.write(value)// to show it in your page.

     }


**notes:**:

  1. some functioncalled built-in function because there are provided from the program language itself.
  2.  you can put function inside function and that's called *Nested-functions* 
 3. make sure to avoid name some functions the same name.it called overriding 

### global and local variables in memory.
 "Each variable that you declare takes up memory.
 
 Global variables use more memory. The browser has to remember them
for as long as the web page using them is loaded. Local variables are only
remembered during the period of time that a function is being executed."


-------------------------------------------


## Reasons for Pair Programming

pair programming is the practice of two developers sharing a same project. 

**Driver and the Navigator**

driver is the persone who setting in front of the computer screen and do everything, typing the code, merge or organized the folder/files.

Navigator is the person who guide the driver. he is like the main brain who understand the issue.

1. Greater efficiency: by divide the effort with each member to decrease the waste-time, error detiction process will be faster

2. Engaged collaboration: increase the experience by both of them will exchange experience and knowledge.

3. Learning from fellow students:working with a teammate can expose developers to techniques they otherwise would not have thought of.

4. Social skills: improve the communication skills because both of them have different thoughts.

5. Job interview readiness: becausethey working together both of them will be ready for any interview questions.

6. Work environment readiness


***resources:***

1. HTML  CSS Design and Build Websites by Jon Duckett.
2. JavaScript and JQuery Interactive Front-End Web Development.
3. [reasons for pair programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)