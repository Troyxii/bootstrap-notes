# ordered notes

primitive and non primitive datatypes 

parseint(num)

string methods: 

length( ): returns the length of the string 

char At(index):Returns the character at a specified index (position)

concat(str):Returns two or more joined strings

endswith(): Returns if a string ends with a specified value

fromcharcode():Returns Unicode values as characters.

Includes():Returns if a string contains a specified value

Indexof():Returns the index (position) of the first occurrence of a value in a string.

Lastindexof():Returns the index (position) of the last occurrence of a value in a string

Match():Searches a string for a value, or a regular expression, and returns the matches

Repeat():Returns a new string with a number of copies of a string.

Replace():Searches a string for a pattern, and returns a string where the first match is replaced

operators in javascript

There are different types of JavaScript operators:
Arithmetic Operators

Arithmetic Operators are used to perform arithmetic on numbers:

Operator	Description

+	                  Addition

-	                  Subtraction

*	                  Multiplication

**	                  Exponentiation (ES2016)

/	                  Division

%	                  Modulus (Division Remainder)

++ 	                  Increment

--	                  Decrement

```jsx
let a = 3;
let x = (100 + 50) * a;
```

Assignment Operators

Assignment operators assign values to JavaScript variables.

Operator	Example	Same As

=	          x = y	 x = y

+=	         x += y	 x = x + y

-=	         x -= y	 x = x - y

*=	         x *= y	x = x * y

/=	         x /= y	x = x / y

%=	         x %= y	x = x % y

**=	         x **= y	x = x ** y

```cpp
let x = 10;
x += 5;
```

Comparison Operators

| Operator | Description |
| --- | --- |
| == | equal to |
| === | equal value and equal type |
| != | not equal |
| !== | not equal value or not equal type |
| > | greater than |
| < | less than |
| >= | greater than or equal to |
| <= | less than or equal to |
| ? | ternary operator |

```cpp
let text1 = "A";
let text2 = "B";
let result = text1 < text2;
```

String Operators

Logical Operators

| Operator | Description |
| --- | --- |
| && | logical and |
| || | logical or |
| ! | logical not |

Bitwise Operators

Bit operators work on 32 bits numbers.

Any numeric operand in the operation is converted into a 32 bit number. The result is converted back to a JavaScript number.

| Operator | Description | Example | Same as | Result | Decimal |
| --- | --- | --- | --- | --- | --- |
| & | AND | 5 & 1 | 0101 & 0001 | 0001 | 1 |
| | | OR | 5 | 1 | 0101 | 0001 | 0101 | 5 |
| ~ | NOT | ~ 5 | ~0101 | 1010 | 10 |
| ^ | XOR | 5 ^ 1 | 0101 ^ 0001 | 0100 | 4 |
| << | left shift | 5 << 1 | 0101 << 1 | 1010 | 10 |
| >> | right shift | 5 >> 1 | 0101 >> 1 | 0010 | 2 |
| >>> | unsigned right shift | 5 >>> 1 | 0101 >>> 1 | 0010 | 2 |

Ternary Operators

Type Operators

array

arrow function:

Arrow functions allow us to write shorter function syntax:

```jsx
let myFunction = (a, b) => a * b;
```

 

```jsx
hello = () => {
  return "Hello World!";
}
```

If you have parameters, you pass them inside the parentheses:

```jsx
hello = (val) => "Hello " + val;
```

anonymous function

It is a function that does not have any name associated with it. Normally we use the *function* keyword before the function name to define a function in JavaScript, however, in anonymous functions in JavaScript, we use only the *function* keyword without the function name.

An anonymous function is not accessible after its initial creation, it can only be accessed by a variable it is stored in as a *function as a value*. An anonymous function can also have multiple arguments, but only one expression.