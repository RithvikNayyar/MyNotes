We are going to use Anaconda in this. For installation you can go to official website.
In vs code we need to create a Conda repository and for that the command 
```
conda create -p venv python==3.12  (version may vary)
```

Syntax refers to the set of rules that defines the combinations of symbols that are considered to be correctly structured programs in a language. In simpler terms, syntax is about the correct arrangement of words and symbols in a code.

Semantics refers to the meaning or the interpretation of the symbols, characters, and commands in a language. It is about what the code is supposed to do when it runs.
Comments in python:
1. For single line comment ## double hash is used
2. For multi line :
```
Hello
```

Python is case sensitive.
```
name="Rithvik"
Name="Nayyar"
print(name,Name)
```

Indentation: Python uses indentation to define the block of code.
Indentation in python is used to define the structure and hierarchy of the code. Unlike many other programming language that use braces {} to delimit blocks of code, python uses indentation to determine the grouping of statements. This means that all the statements within a block must be indented at same level.
```
age = 32
if age>30:
	print(age)
else:
	print("less than 30")
```
Line Continuation: In Python, line continuation is used to break long lines of code into multiple lines for better readability. Here are the two main ways to achieve it:
1) Using a backslash (```\```):
```
total = 10 + 20 + 30 + 40 + 50 + \
        60 + 70 + 80 + 90
print(total)

```
2) Implicit Line Continuation Inside Parentheses, Brackets, or Braces:
```
total = (10 + 20 + 30 + 40 +
         50 + 60 + 70)
print(total)
```
Multiple statements in single line:
```
x=5;y=10;z=x+y
print(z)
```
Semantics in python: In other languages we need to specify what type of data is given example int, float, chat etc., but in python we don't need to specify the type of data we are giving as the kernel automatically understands the data given.
```
#Suppose we take a age.
age = 18
type(age)
print(type(age))
##If you run this python will automatically tell what type of data is given init.
```
**Introduction to variables:** Variables are fundamental elements in programming used to store data that can be referenced and manipulated in a program. In Python, variables are created when you assign a value to them, and they do not need explicit declaration to reserve memory spaces. The declaration happens automatically when you assign a value to a variable. 
```
a=100 ## a is a variable
```
**Declaring and Assigning Variables:** 
```
age = 32
height = 5.9
name = "Krish"
is_student = True

```

















