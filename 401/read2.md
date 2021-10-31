# TDD with Python
TDD stands for: Test Driven Development is an approach in which we build a test first, then fail the test and finally refactor our code to pass the test

**notes:**
- The test file name should follow the same name of module name.
- The cycle is made by three steps:
    1.  Write a unit test and make it fail.
    2. Write the feature and make the test pass.
    3. Refactor the code.

- The greatest advantage about TDD is to craft the software design first


-------------------------------------------


# What does the if __name__ == “__main__”: do?

**notes**
- If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”

- A module is a file containing Python definitions and statements. 

- Python files can act as either reusable modules, or as standalone programs.


----------------------------------


# Recursion

Recursion is the process of defining a problem (or the solution to a problem) in terms of itself. 

you have to be very curful wil recursion cause sometimes it will leads you to an infinite calling (loop) 

recursion like the stack.

for Example: 
if you want to find the great common factor of 5 numbers you can make a function will find the result for 2 numbers and the rest will be passed as parameter and the next number by recursion

**to see more**

[the code](https://drive.google.com/file/d/1NLRcAOy2xhxRLZB12P58NxPX_klwZzOR/view?usp=sharing)



this example i write it when i taked java course


      int r1=GrCoD(1,2);
		int r2=GrCoD(r1,3);
		int r3=GrCoD(r2,4);
		int r4=GrCoD(r3,5);
		System.out.println("The GCD of # is="+r4);
      
      
      public static int GrCoD(int a,int b)
	{
		int gcd=1;
		if(gcd!=0)
		{
			for(int i=1;i<=a && i<=b;i++)
				if(a%i==0 && b%i==0)
					gcd=i;
		}
			return gcd;
		
	}




***resources***
1. [TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)
2. [geeksforgeeks](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)
3. [What on Earth is Recursion? - Computerphile](https://www.youtube.com/watch?v=Mv9NEXX1VHc)
