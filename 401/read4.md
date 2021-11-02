# classes and objects
Python class is like an outline for creating a new object. An object is anything that you wish to manipulate or change while working through the code

Ex:
     
     class Dog:
       pass


An object consists of : 

1. State: It is represented by the attributes of an object.
2. Behavior: It is represented by the methods of an object.
3. Identity: It gives a unique name to an object and enables one object to interact with other objects.


Ex: from geeksforgeeks


       class Dog:
     
           # A simple class
           # attribute
           attr1 = "mammal"
           attr2 = "dog"
 
           # A sample method 
           def fun(self):
               print("I'm a", self.attr1)
               print("I'm a", self.attr2)
 
           # Driver code
           # Object instantiation
           Rodger = Dog()
 
           # Accessing class attributes
           # and method through objects
           print(Rodger.attr1)
           Rodger.fun()


----------------------


# Thinking Recursively in Python

![recursion](https://files.realpython.com/media/python-recursion-title.1beb2deff72a.jpg)
The belief that one has thoughts of one's own is theory of mind about one's self.

recursion is a programming technique using function or algorithm that calls itself one or more times until a specified condition is met at which time the rest of each repetition is processed from the last one called to the first


----------------------


# Python Testing with pytest: Fixtures and Coverage

**notes**

- In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition.
- fixture: are functions attached to the tests which run before the test function is executed
- fixture: provide your test with the appropriate object at the right time.
- You also can decide how often a fixture is run
- if you set the scope of the fixture to be "module", it'll be available throughout your tests but will execute only a single time. You can do this by passing the `scope` parameter to the `@pytest.fixture` decorator
- StringIO(): to convert from string to object
- coverage: to convert code into something human-readable

ex: 


     @pytest.fixture
     def Bob():
        return {"name":"bob"}