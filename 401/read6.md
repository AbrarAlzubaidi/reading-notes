#  How to use the Random Module in Python

## what is random module

 The random module provides access to functions that support many operations.

## some random functions 
1. Randint: random integer number. Randint accepts two parameters: a lowest and a highest number and generate number randomly between them


       import random
       print random.randint(0, 99)


2. Random: If you want a larger number, you can multiply it.


       import random
       random.random() * 100

3. Choice: generate a random value from the sequence sequence.   


       import random
       myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
       random.choice(myList)


4. Shuffle: shuffles the elements in list in place, so they are in a random order.


        from random import shuffle
        x = [[i] for i in range(5)]
        shuffle(x)


5. Randrange: generate a randomly selected element from range(start, stop, step)


        import random
        for i in range(3):
        print random.randrange(0, 101, 5)



-------------------------------


# Risk Analysis

Risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.


**some possible risks that you could encounter**

1. Use of new hardware
2. Use of new technology
3. Use of new automation tool
4. The sequence of code
5. Availability of test resources for the application

**risk magnitude indicators**

1. **High**: means the effect of the risk would be very high and non-tolerable.

2. **Medium**: it is tolerable but not desirable.

3. **Low**: it is tolerable.


**The perspective of Risk Assessment**


1. **Effect** – To assess risk by Effect. In case you identify a condition, event or action and try to determine its impact.

2. **Cause** – To assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach to the point that could be the most probable reason behind that.

3. **Likelihood** – To assess risk by Likelihood is to say that there is a probability that a requirement won’t be satisfied.

**How to perform Risk Analysis?**

1. Searching the risk

2. Analyzing the impact of each individual risk

3. Measures for the risk identified


----------------------------------


# Test-Coverage

**notes**

1. coverage percentage in the upper 80s or 90s means your system is good.
2. why people focus on coverage numbers is because they want to know if they are testing enough.
3. coverage analysis helps you find which bits of your code aren't being tested


----------------------------


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


***Resources***

1. [random module](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
2. [Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)
3. [TestCoverage](https://martinfowler.com/bliki/TestCoverage.html)