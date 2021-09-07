# forms:
1. What is a ‘Controlled Component’?
 by keeping the form data in the component's state. 

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
update the React state, cause state value should updated by user responses

3. How do we target what the user is entering if we have an event handler on an input field?
by `event.target.value` and just call the function.



-------------------------


# The Conditional (Ternary) Operator 

1. A ternary operator allows you to assign one value to the variable if the condition is true.(Shorten your if statements into one line of code )


2. Rewrite the following statement using a ternary statement:
  
  

       if(x===y){
       console.log(true);
       } else {
       console.log(false);
       }




answer:


   x===y ? true : false;

   