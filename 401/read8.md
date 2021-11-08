# List Comprehensions in Python
list comprehensions and how they can be used to write more elegant Python code. offers a shorter syntax when you want to create a new list based on the values of an existing list

Ex: this example from w3school
```
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x for x in fruits if "a" in x]

# we can use if statement inside it  
newlist2 = [x for x in fruits if x != "apple"]
```
**syntax**

`new_list = [ list element seperated by , ]`

## list methods: 
1. Create a List with range()

`lst = [x for x in range(10)]`

2. add elements to list by append()

`lst.append(100)`

3. list comprehensions

`even = [ x for x in range(1,10) if x % 2 == 0]`


----------------------------------


# Primer on Python Decorators
Decorators provide a simple syntax for calling higher-order functions

a decorator is a function that takes another function and extends the behavior of the latter function without explicitly modifying it.

Ex:
 
 ```
 def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

def say_whee():
    print("Whee!")
```

```
# output
>>> say_whee()
Something is happening before the function is called.
Whee!
Something is happening after the function is called.
 ```

**decorate template**

```
def decorate(func):
    @wraps(func)
    def inner(*args, **kwargs):
        # do something before
        ret = func(*args, **kwargs)
        # do something after with ret
        return ret
    return inner

@decorate
def example():
    pass
```

## what can director do 

1. They can be reused.
2. They can decorate functions with arguments and return values.
3. They can use @functools.wraps to look more like the decorated function.