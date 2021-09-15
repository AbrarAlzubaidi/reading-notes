# Understanding the JavaScript Call Stack

![JavaScript-Call-Stack](https://i.stack.imgur.com/xAQPR.png)

1. **What is a ‘call’?**

the call() allows for a function/method belonging to one object to be assigned and called for a different object. call() provides a new value of this to the function/method. With call() , you can write a method once and then inherit it in another object, without having to rewrite the method for the new object.

2. **How many ‘calls’ can happen at once?**

 You can use as many as you want, when function execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

3. **What does LIFO mean?**

Last In First Out 

4. **Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

    
    function firstFunction(){ 

    console.log("Hello from firstFunction");

    }

    function secondFunction(){

    firstFunction();

    console.log("The end from secondFunction");

    }

    secondFunction();


5. **What causes a Stack Overflow?**

is excessively deep or infinite recursion


------------------------------------


# JavaScript error messages

![JavaScript-error-messages](https://wordpress.org/support/files/2020/07/chrome-devtools.png)

1. **What is a ‘refrence error’?**

is the message Excel displays when a formula references a cell that no longer exists

2. **What is a ‘syntax error’?**

is an error in the syntax of a sequence of characters or tokens that is intended to be written in compile-time.
أ

3. **What is a ‘range error’?**

is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value

4. **What is a ‘tyep error’?**

is an error when an operation could not be performed

5. **What is a breakpoint?**

is an intentional stopping or pausing place in a program, put in place for debugging purposes

6. **What does the word ‘debugger’ do in your code?**

allow users to halt the execution of the program, examine the values of variables, step execution of the program line by line


***resources**

Multiple site from **Google**