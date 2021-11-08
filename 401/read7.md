# Python Scope


## The global Statement
 to define a list of names that are going to be treated as global names.

 so when you add it before declaring a variable inside a function scope you make it like a global variable that can any function access it and update it



## The nonlocal Statement
  can be accessed from inner functions, but not assigned or updated. f you want to modify them, then you need to use a nonlocal statement

  Unlike global, you can’t use nonlocal outside of a nested or enclosed function.
   
        >>> nonlocal my_var  # Try to use nonlocal in the global scope
        File "<stdin>", line 1
        SyntaxError: nonlocal declaration not allowed at module level
        >>> def func():
        ...     nonlocal var  # Try to use nonlocal in a local scope
        ...     print(var)
        ...
        File "<stdin>", line 2
        SyntaxError: no binding for nonlocal 'var' found


## globals(): 
**notes**
 - globals() is a built-in function that returns a reference to the current global scope or namespace dictionary.
 - An interesting example of how you can use globals() in your code would be to

    - dynamically dispatch functions that live in the global scope
    - inspect the list of special names in the global scope.
    - you can iterate through it through it using these traditional methods:

           .keys()
           .values()
           .items()


------------------------------------  



# big O

The worst case analysis of algorithm efficiency.


## big O types:
1. O(1): a statement will execute one time
2. O(n): a statement will execute more than one time will execute nth of time.

**notes** 

- n is a integer number 
- usually it descriped loops perfo.

    - ex: Linear Search

3. O(n power of 2,3,4...):usually it descriped nested loops perfo.

     Ex: Bubble Sort, 2D arrays
4. O(2 power of n):usually it descriped recursion 

    like Fibonacci 
5. O(log n):usually it descriped some search algo such as 
 
    binary search
6. O(n log n): usually it descriped some sorting algos such as 

    merge and quick sorts


## big O rules: 

1. different steps get added

if a bit of code big O for it O(n)
the next bit = O(b)
so total big O=O(n+b)


2. drop constant

O(n+3)=O(n)


3. use different variables for different inputs

if array1 of size a
if array2 of size b
loop through each array so big O total= O(a*b) not O(n^2)


4. drop non-dominate terms

if a bit of code big O for it O(n)
the next bit = O(n^2)
so total big O=O(n+n^2)=O(n^2)


---------------------------

***resources***

[python-scope-legb-rule](https://realpython.com/python-scope-legb-rule/)