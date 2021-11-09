# Dunder Methods:
Dunder Methods: names that are preceded and succeeded by double underscores, hence the name dunder. 

Dunder methods let you emulate the behavior of built-in types.

## some Dunder methods: 
1. Object Initialization: `__init__`: To construct objects from the class
2. Object Representation: `__str__`, `__repr__`: 
 
    - the goal of `__repr__` is to be unambiguous 
     - `__str__` the “informal” or nicely printable string representation of an object. 
3. Iteration: `__len__`, `__getitem__`, `__reversed__`: 

     - `__getitem__` like split method
     -`__len__` like len method
     - `__reversed__` like revers method
4. Operator Overloading for Comparing Accounts: `__eq__`, `__lt__`: 

    - `__eq__` like == logic operation
    - `__lt__` like < less than operation

5. Operator Overloading for Merging Accounts: `__add__`: 

    - `__add__` like sum method

6. Callable Python Objects: `__call__`:

    - You can make an object callable like a regular function by adding the `__call__` dunder method.


-------------------------------------


# Basic Statistics in Python — Probability

probability is the measure of the likelihood that an event will occur in a Random Experiment. Probability is quantified as a number between 0 and 1, where, 0 indicates impossibility and 1 indicates certainty. The higher the probability of an event, the more likely it is that the event will occur


## How to calculate the probability of a random variable in a normal distribution in Python

ex from [calculate-the-probability](https://www.kite.com/python/answers/how-to-calculate-the-probability-of-a-random-variable-in-a-normal-distribution-in-python)


        x = 1.0.
        pdf_probability = scipy. stats. norm. pdf(x, loc=0, scale=1)
        print(pdf_probability)
        y = 0.5.
        cdf_probability = scipy. stats. norm. cdf(x, loc=0, scale=1) - scipy. stats. norm. cdf(y, loc=0, scale=1)
        print(cdf_probability)


## What is the method for generating multiple statistics in Python?
statistics. multimode() is introduced in Python 3.8. This function returns the object with the modal value and the number of times it occurs. If there are multiple modal values in the dataset, then only the smallest value is returned


## Z-score
The Z-score is a simple calculation that answers the question, “Given a data point, how many standard deviations is it away from the mean?”

 

## How is Python used in statistics?
Python is a general-purpose language with statistics modules. ... However, when it comes to building complex analysis pipelines that mix statistics with e.g. image analysis, text mining, or control of a physical experiment, the richness of Python is an invaluable asset

***resources**

1. [python-probability](https://www.dataquest.io/blog/basic-statistics-in-python-probability/)
2. [Dunder Methods](https://dbader.org/blog/python-dunder-methods)