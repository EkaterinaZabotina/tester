# JavaSript Operators
1. Arithmetic Operators
2. Assignment Operators
3. Comparison Operators
4. Logical Operators
5. Conditional Operators
6. The typeof Operator
7. Bitwise Operators


**Arithmetic Operators** are used to perform mathematical operations. These operators are frequently used with number 
data types, so they are similar to a calculator. The following example shows how you can use the + operator to add two 
variables together:

let x = 3;
let y = 8;
console.log(x + y); // 11

In JavaScript, we have 8 arithmetic operators in total. They are:

Addition +
Subtraction -
Multiplication *
Division /
Remainder %
Exponentiation **
Increment ++
Decrement --

**Assignment operators** are used to assign a specific value to a variable. The basic assignment operator is marked by 
the equal = symbol, and you've already seen this operator in action before:

let x = 5;

There are 7 kinds of assignment operators that we can use in JavaScript:

|NAME OPERATION            |EXAMPLE |MEANING     |
|Assignment                |x = y   |x = y       |
|Addition assignment       |x += y  |x = x + y   |
|Subtraction assignment    |x -= y  |x = x - y   |
|Multiplication assignment |x *= y	| x = x * y  |
|Division assignment       |x /= y	| x = x /    |
|Remainder assignment	   |x %= y	| x = x % y  |
|Exponentiation assignment |x *= y	| x = x * y  |

**Comparison Operators** are used to compare one value or variable with something else. The operators in this category 
always return a boolean value: either true or false. For example, suppose we want to compare if a variable's value is 
greater than 1. Here's how we do it:

let x = 5;

console.log(x > 1); // true
console.log(x > 7); // false

There are 8 kinds of comparison operators available in JavaScript:

|NAME                  |OPERATION EXAMPLE| MEANING |
|Equal	               |x == y| Returns true if the operands are equal|
|Not equal             |x != y|	Returns true if the operands are not equal|
|Strict equal          |x === y| Returns true if the operands are equal and have the same type|
|Strict not equal      |x !== y| Returns true if the operands are not equal, or have different types|
|Greater than          | x > y |	Returns true if the left operand is greater than the right operand|
|Greater than or equal |x >= y| Returns true if the left operand is greater than or equal to the right operand|
|Less than             | x < y |	Returns true if the left operand is less than the right operand|
|Less than or equal	   | x <= y |	Returns true if the left operand is less than or equal to|

**Logical Operators** are used to check whether one or more expressions result in either true or false.

There are three logical operators available in JavaScript:

|NAME	    |OPERATION|	MEANING |
|Logical AND| x && y  |Returns true if all operands are true, else returns false|
|Logical OR |x || y   |Returns true if one of the operands is true, else returns false|
|Logical NOT|!x	      |Reverse the result: returns true if false and vice versa|

These operators can only return Boolean values. 
For example, we can determine whether '7 is greater than 2' and '5 is greater than 4':

console.log(7 > 2 && 5 > 4); // true
These logical operators follow the laws of mathematical logic:

&& AND operator – if any expression returns false, the result is false
|| OR operator – if any expression returns true, the result is true
! NOT operator – negates the expression, returning the opposite.

**Conditional (Ternary) Operator** is the only JavaScipt operator that requires 3 operands to run.

Let's imagine we need to implement some specific logic in your code. Suppose you're opening a shop to sell fruit. We 
give a $3 discount when the total purchase is $20 or more. Otherwise, you give a $1 discount. We can implement the 
logic using an if..else statement as follows:

let totalPurchase = 15;

let discount;

if (totalPurchase >= 20) {
  discount = 3;
} else {
  discount = 1;
}
The code above works fine, but we can use the ternary operator to make the code shorter and more concise as follows:

let totalPurchase = 15;

let discount = totalPurchase >= 20 ? 3 : 1;
The syntax for the ternary operator is condition ? expression1 : expression2.

**The typeof Operator** is the only operator that's not represented by symbols. This operator is used to check the 
data type of the value you placed on the right side of the operator.

Here are some examples of using the operator:

let x = 5;
console.log(typeof x) //  'number'

console.log(typeof "Nathan") // 'string'

console.log(typeof true) // 'boolean'

console.log(typeof null) // 'object'

console.log(typeof [1, 2, 3]) // 'object'

console.log(typeof {}) // 'object'

console.log(typeof undefined) // 'undefined'

**Bitwise Operators** are operators that treat their operands as a set of binary digits, but return the result of the 
operation as a decimal value.

These operators are rarely used in web development, so you can skip this part if you only want to learn practical 
stuff. But if you're interested to know how they work, then let me show you an example.

A computer uses a binary number system to store decimal numbers in memory. The binary system only uses two numbers, 0 
and 1, to represent the whole range of decimal numbers we humans know.

For example, the decimal number 1 is represented as binary number 00000001, and the decimal number 2 is represented as 00000010.

**Динамическая типизация** — приём, используемый в языках программирования, при котором переменная связывается с типом в момент присваивания значения, а не в момент объявления переменной. JavaScript - это как раз пример языка с 
динамической типизацией. Такое поведение отличает JS от некоторых других языков программирования, где тип переменной должен быть объявлен заранее и не может изменяться во время работы программы.