### What is Python?
Python is a dynamically typed, General Purpose Programming Language that supports an object- oriented programming approach as well as a functional programming approach.
Python is also an interpreted and high-level programming language.
It was created by Guido Van Rossum in 1989.
It is a very powerful language, is portable, has built-in object types, many libraries and is free.

**Features of Python:** 
* Python is a simple and easy to understand 
* it is interpreted and platform-independent which make dubbing very easy 
* python is a open source language
* python provides very big library support some of the popular libraries include NumPy, Tensor flow, Selenium, OpenCV etc.
* it is possible to integrate other programming language within python.

**What is Python used for?**
* Python is used in Data visualization to create plots and graphical representations.
* python helps in data analytics to analyze and and understand raw data for insights and trends.
* it is used in AI and Machine Learning to simulate human behaviour and to learn from past data without hard coding.
* it is used to create web applications
* it can be used to handle databases
* it is used in business and accounting to perform complex mathematical operations along with quantitative and qualitative analysis.
![[Python-20240905045112766.webp|466]]
**What is a syntax?**
Syntax is the arrangement of words and phases to create well-formed sentences in a language, in the case of a computer language, the syntax is the structural arrangement of comments, variables, numbers, operators, statements, loop, functions, classes, object, etc., which helps us to understand the meaning or semantics of a computer language.

**Writing first line of code:**
In python we don't need to write main function to execute the code we can directly print in the ide.
```
print("Hello World!")
print('Hello world!')
```
Just copy and paste the code and you will see the miracles of python.
In python we can print a string using a ( " ) or ( ' ), means using double quote or single quotes.

**Python Comments:** A comment is a part of the coding file that the programmer does not want to execute, rather the programmer uses it to explain a block of code or to avoid the execution of a specific part of code while testing.
```
# in hash what ever we write will not be executed when i goto next line

print("Hello world!")  # now print statement will be executed but not what i have written after the hash.
```
In the above block of code i used # which comments out a single line of code.
There is a way to do multi-line comments also.
```
""" In python we can use 3 double quotes to comment out multiple lines of code.
Remember what ever you type in this will not be printed how many lines it may be.
To exit out of this we need to use triple quotes again and thats it we are out of comments and below this everything will be executed."""
print("Hello world!")
```
##### Python Variable:
Variables are containers that store information that can be manipulated and referenced by the programmer within the code.
In python , the programmer does not need to declare the variable type explicitly, we need to assign the value of the variable.
```
name = "Rithvik"	#type string
age = 23			#tpye integer
passed = True		#type boolean
```

It is always advisable to keep variable names descriptive and to follow a set of convections while creating variables:
* Variable names can only contain alpha-numeric characters and underscores
* Variable name must start with a letter or the underscore character.
* Variable are case sensitive.
* Variable name cannot start with a number.
```
Color = "yellow"    #valid variable name
cOlor = "red"       #valid variable name
_color = "blue"     #valid variable name

5color = "green"    #invalid variable name
$color = "orange"   #invalid variable name
```
Sometimes a multi-word variable name can be difficult to read by the reader. To make it more readable, the programmer can do the following:
```
NameOfCity = "Mumbai"       #Pascal case
nameOfCity = "Berlin"       #Camel case
name_of_city = "Moscow"     #snake case
```
**Scope of the Variable:** The scope of the variable is the area within which the variable has been created. Based on this a variable can wither have a local scope or a global scope. 

**Local Variable:** A local variable is created within a function and can be only used inside that functions. Such a variable has a local scop.
**Global variable:** A global variable is created in the main body of the code and can be used anywhere within the code. Such a variable has global scope.
```
icecream = "Vanilla" 		# icecream is global variable
def foods():
	fruit = "Lichi"
	vegetable = "Potato"	#fruit and vegetable are local variable
	print(vegetable + " is a local variable value.")
	print(fruit + " is a local variable value.")
	print(icecream + " is a global variable value.")
foods()
```

##### Data types
 Data type specifies the type of value a variable requires to do various operations without causing an error. By default, the python provides the following built-in data types:
**Numeric data: int, float, complex**
 Int 3,-8,0
 Float: 7.349,-9.0
 Complex: 6 + 2i 
**Text data: str:**
 str: "Hello world!!!", "Python Programming"
**Boolean data:**
 Boolean data consists of values of true or false.
**Sequenced data: list, tuples, range**
 List: A list is an ordered collection of data with elements separated by a comma and enclosed within square brackets. Lists are mutable and can be modified after creation.
 ```
 list1 = [8,2.3,[-4,5],["apple","banana"]]
 print(list1)
 ```
 Output:
 ```
 [8, 2.3, [-4, 5], ['apple', 'banana']]
 ```

Tuple: A tuple is an ordered collection of data with elements separated by a comma and enclosed within parentheses. Tuples are immutable and can not be modified after creation.
```
tuple1 = (("parrot","sparrow"),("Lion","Tiger"))
print(tuple1)
```
Output
```
(('parrot', 'sparrow'), ('Lion', 'Tiger'))
```
**Range:** Range returns a sequence of numbers as specified by the user. If not specified by the user then it starts from 0 by default and increments by 1.
```
sequence1 = range(4,14,2)
for i in sequence1:
	print(i)
```
**Mapped data: dict**
Dict: a dictionary is an unordered collection of data containing a key: value pair. The key: value pairs are enclosed within curly brackets.
```
dict1 = {"name":"sakshi", "age":20, "canvote":True}
print(dict1)
```
Output:
```
{'name': 'Sakshi', 'age': 20, 'canVote': True}
```

To be continued...
Test 1 - 29 dec
Test 2 - 29
Test - Windows

Hello

Test 4 