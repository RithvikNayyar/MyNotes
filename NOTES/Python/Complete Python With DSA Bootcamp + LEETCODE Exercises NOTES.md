We are going to use Anaconda in this. For installation you can go to official website.  Udemy. Ipynb file is also available in this directory.
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
a, b = 1, 2,  
print(z,a,b)
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

In simple word variables are in named storages in which data is stored.
```
a=100 ## a is a variable
```
**Declaring and Assigning Variables:** 
```
age = 32
height = 5.9
name = "Krish"
is_student = True

##printing the variable

print("age :", age)
print("Height:",height)
print("Name:",name)
```
**Naming Conventions:** variable name we describe should be descriptive. They must start with a letter or an ```_``` and contain letters, numbers and underscores. It helps you or others understand the code better and avoids confusion and errors.

__Key rules in Python__ :
```
1. Variables and functions we use snake case:  
- we define variables with All lowercase letters with underscores(_) separating words. ex: user_age, calculate_sum.  
- indicates variables or functions that store data or perform actions.  
2. Classes are defined with pascal case:  
- pascal case is to capitalize the first letter of each word, no spaces or underscores. ex: StudentRecord, CarModel.  
- It means we created blueprints or represents structures or templates for creating objects.
3. Constants:  
- constants are the values which do not change or are not meant to be changed during execution of a program. They represent fixed values, limits or keys.  
- It is written in all Uppercase letters with underscores separating words. ex: API_KEY, MAX_LIMIT.  
4. Private Names:  
- Starts with a single underscore(_). Ex: _secret_data, _helper_function.  
- Purpose: Indicates names intended for internal use (Not a part of public api key).  
5. Special methods:  
- Uses double underscore (__). Example __inti __, __str __. Reserved methods with special meaning in python.
```
**Why follow these rules?
* Readability: Makes codes easier to understand.  
* Consistency: Helps you and others follow the same style.  
* Avoid Errors: Prevents conflicts with Python's Reserved keywords or built-in-Names.
```
## Valid Variable Name  
First_Name = "Rithvik"  
Last_Name = "Nayyar"
```
```
# Invalid variable names  
#first-name="Krish"  
#2age=30  
##@name="Krish"
```











