# components

## what is the component?
a small piece of code that fills a certain part of the user interface. is a software object.

**A component can have three different views**

1. Object-oriented view
2. Conventional view
3. Process-related view

## what is the characteristics of Components
1. Reusability 
2. Replaceable 
3. Not context specific 
4. Extensible 
5. Encapsulated 
6. Independent


## what is the advantages of component
1. Ease of deployment and handel.

2. Reduced cost: because it easy to handel and deployment.

3. Ease of development: by allowing development without impacting other parts of the system.

4. Reusable: they can be used to spread the development and maintenance cost .

5. Modification of technical complexity: by using its container and its services.

6. Reliability: The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

7. System maintenance and evolution: Easy to change and update the implementation without affecting the rest of the system. just maintane the specific part.

8. Independent: each component have its own function.


-------------------------------------------------------



# React
React is a JavaScript library for building modern applications. React is used for handling the view layer. its typed like tags

**notes**:

- A component takes in parameters, called props: ('div')

- simple EX: 
   
         ReactDOM.render(
           <h1>Hello, world!</h1>,
               document.getElementById('root')
            );


its calling the div element in HTML file by its ID and print `Hello world` in the page. using ReactDOM.render

- JSX produces React “elements
   Ex:

        const element = <h1>Hello, world!</h1>;


-  you can use JSX inside of if statements and for loops, assign it to variables, accept it as arguments, and return it from functions
- you can specifying atributes by using `" "` or `{ }`
- you can render element using React by declare it then render it by its id, class, ...
- you can define a component by using functions ar classes
- Props are Read-Only