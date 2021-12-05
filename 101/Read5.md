
## operations in JS:

** JS has many type of operators,such as:**

1. Assignment operators (=): 

it's assigned thw value for the left operator depends on the value of the right one.it a binary operator.

2. Comparison operators (===)(!==)(==)(!=)(<)(<=)(>)(>=):

compares its operands and returns a logical value. it ial a binary operator.

3. Arithmetic operators(+)(-)(*)(/):
takes numerical values.some of them is a binary operator like (+)(-)(*)(/)(%)(**). the other is a unary operator like (++)(--) (+x)(-x)

4. Bitwise operators(&)(|)(~)(^)(<<)(>>)(>>>):

reats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers.(~)  is only the unary operator. 

5. Logical operators(&&)(||)(!)

used with Boolean (logical) values they return a Boolean value.(!) is only the unary operator. 

6. String operators

7. Conditional (ternary) operator

is the only JavaScript operator that takes three operands.

**SYNTAX:** condition ? val1 : val2

Copy to Clipboard
If condition is true, the operator has the value of val1. Otherwise it has the value of val2

8. Comma operator

evaluates both of its operands and returns the value of the last operand
 This operator is primarily used inside a for loop, to allow multiple variables to be updated each time through the loop. 

9. Unary operators
 - The delete operator deletes an object's property also it can delete array elements.
  - The typeof operator returns a string indicating the type of the unevaluated operand.

10. Relational operators
  - The in operator returns true if the specified property is in the specified object
  - he instanceof operator returns true if the specified object is of the specified object type

some of them calld **Binary operators** which requires two operands, one before the operator and one after the operator. the others calld **Unary operators** which equires a single operand, either before or after the operator.

### Destructuring:
makes it possible to extract data from arrays or objects using a syntax that mirrors the construction of array and object literals.
*for EX:*

var foo = ['one', 'two', 'three'];

// without destructuring that means we have to declare for each variable an element of array (multi-instruction) if array's size too big it could be wasted time if we use this way.

var one   = foo[0];
var two   = foo[1];
var three = foo[2];

// with destructuring: we can save time and have the same result (one instruction much better) 
var [one, two, three] = foo;


--------------------------------------------
## loops:
Loops offer a quick and easy way to do something repeatedly. 

**The statements for loops provided in JavaScript are:**

1. for statement:

A for loop repeats until a specified condition evaluates to false

**EX:**
for (var x=1; x<=4; x++){

  //do something
}
 
2. do...while statement

The do...while statement repeats until a specified condition evaluates to false.

3. while statement

A while statement executes its statements as long as a specified condition evaluates to true

**EX**
while (n < 3) {

  //do something

  n++;}

4. labeled statement
5. break statement

to terminate a loop, switch, or in conjunction with a labeled statement.

6. continue statement
7. for...in statement
8. for...of statement
