## execution content types:
1. global context: not inside function or any curly prackets.
2. function context: any statement inside the function.
3. eval context: inside any eval function.


## varible scope:
1. global scope: when the variables are outside the function or any curly prackets.
2. function scope: when the variables are inside the function.


**stack mathod means** when a statement has the a priority to execute first it will execute even if this statement at the last line in the code.

***First In First On*** first statement execution will be execution first.

### prepare:
like variable or function when its turn comes, like when we create a variable without using it [it still wait its turn].


### execute:
when you assign a value to a variable and use it somewhere.

## scope:
each scope has its own variable. in nested scopes inner-scope can access the outer-scope varibles. but the opposite is not.


## when error happens it will show you on console msg have:
1. the type of execution.
2. name of the file that hold errors.
3. line number that holds error.


### error types:
1. syntax error: you write somrthing incorrectly.ex: if you miss the `)` closing parentheses.

2. reference error: if you not declared somrthing and you use it. ex:

        console.log(name); // name not declared before.


3. URL error: if some symbols appears in the link. ex:

        ?   &   #   :   ;   /

4. eval error: incorrect use of eval function.
5. type error: if you type somrthing wrong. ex:

        consol.log();  // e charectar is missing.

6. range error: if you call somrthing/ print/ execute outer of range. ex:

             let array=[1,2,3];
             array[3]=5;// 3 is not of range of index.

7. NAN error: not a number.ex:

              var x= 5*'d';


## you can trace errors by your self before using tools.
1. try to narrow the area where the error may to be? by tracing it viuially. 
2. now you can use tools after narrowing the area of code. use tools to write msg to tell you how far the code is running.
3. use breakpoint where things are wrong.
4. divide the error code into smull one to make it easies to you.


## what is the tools may you use to decate the errors:
1. console: you can `console.log` where you think could be an error and watch the console window if it appears an error msg or not.
2. breakpoint: by make the code stop when specific line (that you determine it) comes. it make error detection process much easier.
3. try, catch and finally:


     try{
       // block of code will run if there is no error/ exception.
     }catch(exception){
       // code will run if there an error.
     }
     finally{
       // code will run either try or catch runs.
     }
          

 ***resources:***

1. JavaScript and JQuery Interactive Front-End Web Development.