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
       
--------------------------------------------
## Control flow:

means that when you read a script, you must not only read from start to finish (line by line in normal way) but also look at program structure and how it affects order of execution.*it caused by condition statements and loops*

so in normal way code runs from first instruction to the next one (line by line) some instruction may you jump to (for example) to the last line for execute somthing, get the result then back to the line. the statements which make this happen is loop and conditional statements. 
     
 



