# flow control

## Python Flow Control

In Python, flow control refers to the way the program's execution is directed based on certain conditions. Python provides several flow control statements, including:

- **If Statements**: Used to perform different actions based on different conditions.
- **For Loops**: Used to iterate over a sequence of elements.
- **While Loops**: Used to repeatedly execute a block of code as long as a specified condition is true.
- **Break and Continue Statements**: Used to alter the flow of a loop.
- **Try and Except Statements**: Used for error handling.

These flow control statements allow developers to control the execution of their Python programs and make them more flexible and efficient.

- **For Loops**: Used to iterate over a sequence of elements. It allows you to execute a block of code for each item in a sequence, such as a list or a string.

Here's an example of a for loop in Python:

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

```

This loop will iterate over the `fruits` list and print each item on a separate line.

For loops are commonly used when you want to perform a certain operation on each item in a collection or when you want to repeat a block of code a specific number of times.

- **If-Else Statements**: Used to perform different actions based on different conditions. It allows you to specify a block of code to be executed if a certain condition is true, and another block of code to be executed if the condition is false.

Here's an example of an if-else statement in Python:

```python
age = 18
if age >= 18:
    print("You are eligible to vote!")
else:
    print("You are not eligible to vote!")

```

In this example, if the `age` variable is greater than or equal to 18, the program will print "You are eligible to vote!". Otherwise, it will print "You are not eligible to vote!".

If-else statements are useful when you want to perform different actions based on different conditions or make decisions in your program based on certain criteria.

- **If-Elif-Else Statements**: Used to perform different actions based on multiple conditions. It allows you to specify multiple blocks of code, each associated with a specific condition. If the first condition is not met, it moves on to check the next condition until a condition is met or the final else block is reached.

Here's an example of an if-elif-else statement in Python:

```python
score = 85
if score >= 90:
    print("You got an A!")
elif score >= 80:
    print("You got a B!")
elif score >= 70:
    print("You got a C!")
else:
    print("You need to study harder!")

```

In this example, the program checks the value of the `score` variable and prints a corresponding message based on the score. If the score is 85, it will print "You got a B!".

If-elif-else statements are useful when you have multiple conditions to check and want to perform different actions based on those conditions.