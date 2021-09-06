# lists and keys:
**notes:**

1. list usually will be render inside a component
2. key is a special string attribute you need to include when creating lists of element
3. Keys help React identify which items have changed, are added, or are removed.
4. Keys used within arrays should be unique among their siblings.

**questions**
1. What does .map() return?
return modified array.

2. If I want to loop through an array and display each value in JSX, 
 how do I do that in React?
 
      arr.map(value=>{
        return <li>{value}</li>
      })

3. Each list item needs a unique

 _key_.

4. What is the purpose of a key?  
Keys help React identify which items have changed, are added, or are removed.



---------------------------------------

# Spread Operator (…) in JavaScript:

**notes:**

1. ***the usage***: adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
2. One of the benefits of using the spread operator is that it will create a new reference to its primitive values, copying them. SO it means *changes to the original array will not affect the copied array*
3. the most helpful usage of spread operator when combining arrays such as when adding an item to React State.


**questions:**

1. What is the spread operator?
it is the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.


2. List 4 things that the spread operator can do.
Copying an array, Concatenating or combining arrays, Using Math functions, Using an array as arguments.

3. Give an example of using the spread operator to combine two arrays.


    const array1 = [`hello `,`world `,`! `]
    const array2 = [`it `,`is `,`perfect `]
    const array3 = [...array1,...array2]
    console.log(...array3) // it will print--> hello world ! it is perfect 


4. Give an example of using the spread operator to add a new item to an array.


     const numbers = ['1','2','3','4','5']
     const numberCopy = [...numbers];
     numbers[0] = '0'
     console.log(...[...numbers,...numberCopy]) //it will print --> 012345


5. Give an example of using the spread operator to combine two objects into one.

 

      const firstObj = {Fname: "abrar"}
      const secondObj = {Lname: "alzubidi"}
      const combineObj = {...objectOne, ...objectTwo}
      console.log(combineObj) // will print--> {Fname: "abrar", Lname: "alzubaidi" }



---------------------------------------------------------



# How to Pass Functions Between Components?
like the properties Ex:


  at render in the class when pass the property we do this 

    `name={name}`

  so function it simmilar of this 

  when you declared a function you can pass it like:

    `nameFunction={this.nameFunction}`

  and you can use it in another component like:

    `this.props.nameFunction`
      

**questions:**

1. In the video, what is the first step that the developer does to pass functions between components?
declare the function with parameter 'name' to pass it to the function and check the name then change the 'count' depened on the name. then loop throw the objects and check the name then increment the count

2. In your own words, what does the increment function do?
it will increment the number of clicks 'that beside the name' when the button is clicked.

3. How can you pass a method from a parent component into a child component?
like this `nameFunction={this.nameFunction}`

4. How does the child component invoke a method that was passed to it from a parent component?
like this `this.props.nameFunction`
      