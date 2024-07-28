
YOUTUBE LINK: https://bit.ly/50HRCP, https://bit.ly/CWCWH10HR
## Basic of computing

##### What is a computer?
Computer is a device which compute data.

Data can be:
1) Binary Data (0,1)  - Digital computer 
2) Physical phenomena (like speed, temp, pressure)  - Analog Computer
* Another type is hybrid computer which is Digital + Analog computer

#### Digital Computer
* Digital computer is a electronic machine which accept data in input, process it & produce information in output.
* They work on Bit()
* Input data is first converted to binary data then the output is given.(Text, video, image, audio)
* Advantages:
1) Accuracy
2) speed
* Disadvantages: Cannot calculate physical phenomena
![[Mynotes/C/c all pictures in notes/Pasted image 20240715094151.png]] 

#### Analog Computer
* They work on physical phenomena - Advantage
* They are less accurate & slow - Disadvantage
Ex: Speedometer, Voltage meter, Pressure gauge, etc. 

#### Hybrid computer
* It has some portion of digital computer & Analog Computer (ex: Digital speedometer, Digital thermometer, Electric multimeter)
__________________________________________________________________________
![[Mynotes/C/c all pictures in notes/Pasted image 20240715094407.png]]
![[Mynotes/C/c all pictures in notes/Pasted image 20240715094454.png]]
![[Mynotes/C/c all pictures in notes/Pasted image 20240715100243.png]]
* Note: The Above pictures shows the types of devices, Ac - Dc current & How computer reads binary number in system.

##### How does a Digital computer work
* In a digital computer lot of calculations goes on In ALU (Arithmetic Logic Unit) which performs all the work.
1) Arithmetical Operations : ( +, -, * , / )
2) Logical Calculations : (< , > , == , AND, OR )
* Arithmetic Logic Unit get all the commands from Control unit (CU) & performs all the task
* When they are combined together they are called CPU (Central Processing Unit)
* CPU takes data from input/output devices, storage devices(Hard disk drive)(Music, video) 
* CPU doesn't have direct link to HDD, if it were then as soon as it reads the data then it would run it without permission or directly open all files as soon as reads HDD.
* To over-come this issue there is a temporary Memory called RAM, So first the data is sent to ram then it runs on the system.
![[Mynotes/C/c all pictures in notes/Pasted image 20240715105723.png]]

#### Software & It's Development
* Software either control hardware or do some specific task
* Software is a set of instructions written in specific computer understandable form to perform specific task.
* EX: When you are on a desktop and type something like your name but nothing happens and then you open a notepad and type your name then you see your name on the notepad. So this show that I/O devices are controlled through software.
![[Mynotes/C/c all pictures in notes/Pasted image 20240715111547.png]] 

##### How to develop a software
* For developing a software you need to know a programming language (c, c++, java, python)
* We need a translator for the language like compiler which changes our code to binary language so that out system understands.

#### Computer programming languages
##### Computer Language
* Language which is understand by the computer is called computer language or it is called Machine language(ML).
* Computer can only understand 0 or 1, so it means machine language only has two digits 0 or 1.
* We cannot write in Machine language as it is Complicated and Binary number vary computer to computer.
##### Programming Language
* Language in which we can design software/program for computer is called Programming Language (PL).
* Programming Language provide us with set of instructions to computer to execute. Set of instructions is called Software Program.
* The process of writing program is called Programming.
* The person who develops the software called software developer.
 
 Programming language are of 3 types:
1)  Low Level Language:
* Those Language which are close to hardware or hardware friendly.
* Commands or function map closely to processor instructions.
* Program written in low-level languages tend to be relatively non-portable, due to being optimized for a certain type of system architecture. It is machine dependent,
* programs written in low level language can be made to run very quickly, with a small memory footprint.
* It needs assembler for translation.

2) Middle level language :
* A middle-level programming language serves as a bridge between high-level and low-level languages.
- It strikes a balance: more abstraction than low-level languages (making code easier to write and understand) and more control and efficiency than high-level languages.
- These languages aim for better performance than high-level languages. They allow manual memory management and direct access to hardware resources.
- **Examples**: C and C++ are often considered middle-level languages. They offer features from both high-level languages (like structured programming) and low-level languages (like direct memory manipulation).
- Middle-level languages are suitable for system programming, embedded systems, and performance-critical applications.
- They allow you to write efficient code while maintaining a reasonable level of developer productivity.

3) High Level Language :
*  Those language which are close to programmer or programmer friendly.
* It may use natural language element such as alphabet, numerical, etc., be easier to use, or may automate significant areas of computing system(Memory management), making the process of developing a program simpler and more understandable than when using a lower-level language.
* Programs written in high - level languages tend to be relatively portable.
* They do not provide many facilities at hardware level.
*  A Program written in a low level language can be made to run very quickly, with a small memory footprint.
* it needs compiler or interpreter for translation.

#### Language Translator 
A translator or programming language processor is a generic tern that can refer to software that converts code from one language to another. Follow diagram below...
![[Mynotes/C/c all pictures in notes/Pasted image 20240716070523.png]]

##### Assembly Language and Assembler
###### Assembly Language 
- Assembly language is a low-level programming language.
- It uses mnemonic codes (short, human-readable instructions) to represent machine language instructions.
- Each instruction corresponds directly to an operation the computer’s CPU can perform.
- Programmers write assembly code in a text editor.
- Assembly language is closer to machine code than high-level languages like C++ or Java.
- It allows direct access to hardware resources (memory, I/O ports).
- Ideal for systems programming and device drivers.
###### Assembler
- An assembler is a specialized software tool.
- It converts assembly code into machine language (binary code) that the CPU can execute.
- Assemblers play a crucial role in translating human-readable assembly instructions into executable machine code.
![[Mynotes/C/c all pictures in notes/Pasted image 20240716071718.png]]

##### Compiler & Interpreter
- A translator or programming language processor is a generic term that can refer to anything that converts code from one computer language into another.
- Compiler and interpreter are translator for high level Language.
![[Mynotes/C/c all pictures in notes/Pasted image 20240716073124.png]]

| COMPILER                                                                                                                                                                                                                           | INTERPRETER                                                                                                                                                                                                                             |
|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| - Translates high-level code into machine code ahead of time.<br>- Produces an executable program.<br>- Checks for syntax and some semantic errors.<br>- Compiled code runs faster.<br>- Examples: GCC (for C/C++), Java compiler. | - Translates code line-by-line during program execution.<br>- No separate executable; always needs the interpreter.<br>- Easier to debug.<br>- Interpreted code runs slower.<br>- Examples: Python interpreter, JavaScript interpreter. |
##### What is IDE(Integrated Development Environments)?
- **All-in-One Workspace**: IDEs combine essential tools (source-code editors, debuggers, build automation) into a single environment.
- **Boosted Productivity**: IDEs catch syntax errors as you type, provide code completion, and offer refactoring tools.
- **Language-Specific IDEs**: Different IDEs cater to specific languages (e.g., Visual Studio for .NET, PyCharm for Python).

__________________________________________________________________________
**I CHOSE DEV C++ FOR MY IDE YOU MAY CHOOSE WHICH EVER YOU FEEL COMFORTABLE AS THE RESULTS WILL BE SAME.
__________________________________________________________________________

## C Programming 
### CHAPTER 1
##### IDE that i use
For C programming i used Dev C++ or VS code. Dev C++ comes with inbuilt compiler so you can directly install and go, But i recommend you to install code blocks or VS code as its updated frequently and get more plugins. All the links are down below.
Dev C++ LINK:  https://sourceforge.net/projects/orwelldevcpp/
Code blocks LINK: https://www.fosshub.com/Code-Blocks.html
VS code LINK: https://code.visualstudio.com/

#### First Program in C language
After installation of your ide create one project and name it as you wish then write your first program.
**Printing Hello world
```
#include<stdio.h>
void main ()
{
	printf("Hello World");
}
```
OUTPUT: Hello world
![[Mynotes/C/c all pictures in notes/Pasted image 20240716084721.png]]
***
The above code is also called Boiler plate code.
*** 

#### History of C Language and Standards 
1. **Early C (1969)**:
    
    - **Birth of B**: C’s roots trace back to an earlier language called **B**, which was developed by Dennis Ritchie at Bell Laboratories. B itself was based on languages like **BCPL** and **CPL**.
    - **Typeless Beginnings**: In its early days, C remained a typeless language, akin to its predecessor BCPL. It was created to replace the PDP-7 assembler as the system programming language for Unix.
    - **Operators and Evolution**: B introduced operators like `++`, `--`, and compound assignment. However, it lacked explicit types.
2. **Standardization Efforts**:
    
    - In 1983, the **American National Standards Institute (ANSI)** established a committee called **X3J11** to standardize the C language.
    - This marked a pivotal moment—the transition from an evolving language to a well-defined standard.
3. **C89 (ANSI C)**:
    
    - In 1989, the first official standard for C was published: **ISO/IEC 9899:1990**, commonly known as **C89**.
    - Key features included:
        - Introduction of `volatile`, `enum`, `signed`, and `void`.
        - Influence from C++: concepts like `const` and function prototypes.
4. **Subsequent Standards**:
    
    - **C90**: The ANSI C standard was accepted as an international standard by ISO/IEC in 1990.
    - **C99**: The 1999 standard brought significant enhancements:
        - `bool`, `long long`, `<stdint.h>`, variable-length arrays, designated initializers, and more.
        - Hexadecimal floating-point format (`%a`), complex numbers, and the `__func__` identifier.
        - Removal of implicit functions and implicit `int`.
5. **Recent Updates**:
    
    - **C11**: The 2011 standard (ISO/IEC 9899:2011) introduced concurrency support and other improvements.
    - **C17**: A minor update (ISO/IEC 9899:2018) with bug fixes.
    - **C23**: The ongoing work toward the next standard.

And there you have it—a glimpse into the evolution of C, from its humble beginnings to its status as a foundational language for systems programming, embedded systems, and more!

#### Properties of C Language

1. C is a high level programming language having features of low level programming language.
2. Permissive language (Easily controllable)
3. Efficiency 
4. Portability (The main reason why c is build)
5. Flexibility
![[Mynotes/C/c all pictures in notes/Pasted image 20240717080151.png|277]]

#### How to write C Program
##### Rules for making C
1. C is a functional programming language. (Function is a set of statement which perform some action)
![[Mynotes/C/c all pictures in notes/Pasted image 20240717082009.png|652]]
2. C program require at least one function.
3. C program require main() to run.
4. Every program starts with main() and ends with main().
5. C program not allow functions in side function.
6. In C program, One function can call another function.
7. Declaration of function in C.
8. C supports two types of function.
9. C is a Case sensitive language
10. C program requires compiler to develop.

#### Variables
A variable is a container which stores a ‘value’. In kitchen, we have containers storing Rice, Sugar etc. Similar to that, variables in C stores value of a constant.
(hindi-english: simply, it is name of the memory location. Variable ek memory location ka naam hai).
![[Mynotes/C/c all pictures in notes/Pasted image 20240717100150.png]]
![[Mynotes/C/c all pictures in notes/Pasted image 20240717101015.png|459]] 

##### RULES FOR NAMING VARIABLES IN C 
1. First character must be an alphabet or underscore (_) 
2. No commas, blanks are allowed. 
3. No special symbol other than (_) allowed. 
4. Variable names are case sensitive. 

We must create meaningful variable names in our programs. This enhances readability of our programs.

#### CONSTANTS 
An entity whose value does not change is called as a constant. A variable is an entity whose value can be changed. 

##### TYPES OF CONSTANTS 
Primarily, there are three types of constants: 
1. Integer Constant → 1,6,7,9 
2. Real Constant → 322.1, 2.5 ,7.0 
3. Character Constant → ‘a’, ‘$’, ‘@’ (must be enclosed within single quotes)

#### KEYWORDS 
These are reserved words, whose meaning is already known to the compiler. There are 32 keywords available in C.
![[Mynotes/C/c all pictures in notes/C all in 1 notes-20240717102323564.webp]]

#### COMMENTS

Comments are used to clarify something about the program in plain language. It is a way for us to add notes to our program. There are two types of comments in C. 
1. Single line Comment: Single-line comments start with two forward slashes (//). Any information after the slashes // lying on the same line would be ignored (will not be executed).
```
// this is single comment
```

2. Multi-line Comment: A multi-line comment starts with /* and ends with */. Any information between /* and */ will be ignored by the compiler.
```
/* 
This is a multi-line comment 
*/
```

#### COMPILATION AND EXECUTION
- A compiler is a computer program which converts a C program into machine language so that it can be easily understood by the computer. 
- A C program is written in plain text. 
- This plain text is combination of instructions in a particular sequence. The compiler performs some basic checks and finally converts the program into an executable.
![[Mynotes/C/c all pictures in notes/C-20240724152136590.webp]]
#### LIBRARY FUNCTIONS
C language has a lot of valuable library functions which is used to carry out certain tasks. For instance printf() function is used to print values on the screen.
```
include <stdio.h> 
int main() 
{ 
int i = 10; 
printf("This is %d\n", i); 
// %d for integers 
// %f for real values (floating-point numbers) 
// %c for characters 
return 0; 
}
```

##### TYPES OF VARIABLES
 1. Integer variables → int a=3; 
 2. Real variables → int a=7; float a=7.7; 
 3. Character variables → char a= ‘b’;

#### RECEIVING INPUT FROM THE USER
In order to take input from the user and assign it to a variable, we use scanf() function.
**SYNTAX:
```
scanf("%d",&i);
```
![[Mynotes/C/c all pictures in notes/C-20240724153621701.webp]]
- ‘&’ is the “address of” operator and it means that the supplied value should be copied to the address which is indicated by variable i.

#### Chapter 1 Practice set
*** Just in case if you don't know the formula you can always use the help of chatgpt
1) write a C program to calculate area of rectangle:
		a. Using hard coded inputs
		b, Using inputs supplied by the user.
SOL:  1.a Solution
```
#include<stdio.h>
int main ()
{
    int length, width, area;
    length = 5;
    width = 6;
    // As we know area of a rectange is a = lxb so...
    area=length*width;
    printf("Area of a rectangele is %d", area);
    return 0;
}
// output for this is a=5*6 = 30, Area of a rectangele is 30
```
SOL: 1.b Solution
```
#include <stdio.h>
int main()
{
    int length, width, area;
    printf("Enter length: ");
    scanf("%d", &length);
    printf("Enter width: ");
    scanf("%d", &width);
    area = length * width;
    printf("Area of a rectangle is %d\n", area);
    return 0;
}
//output for this depends on the input you have given
```

2)  a. Calculate the area of a circle.
	b. modify the same program to calculate the volume of a cylinder given its radius and height.
SOL: 2.a&b Solution
```
#include <stdio.h>
int main()
{
    int r, h;
    float area, volume;
    printf("Enter radius: ");
    scanf("%d", &r);
    printf("Enter height: ");
    scanf("%d", &h);
    // pie value is 3.14...  or 22/7 anything you take values are the same
    area = 3.14 * r * r;
    volume = 3.14 * r * r * h;
    printf("Area of a circle is %f\n", area);
    printf("Volume of circle is %f\n", volume);
    return 0;
}
// for output i took r =5 h = 10 so area = 78.5 and volume = 785
```

3) Write a program to convert Celsius (Centigrade degrees temperature to Fahrenheit).
SOL: Solution: As i don't know the formula to convert Celsius to Fahrenheit so i am going to use chatgpt and it gave me a answer I.e., F = C X 9/5 +32 soo....  
```
#include <stdio.h>

int main() {
    float celsius, fahrenheit;
    printf("Enter temperature in Celsius: ");
    scanf("%f", &celsius);
    fahrenheit = (celsius * 9 / 5) + 32;
    printf("%.2f Celsius = %.2f Fahrenheit\n", celsius, fahrenheit);
    return 0;
}
// here %.2f will print a floating-point number up to two places after the decimal
```

4) Write a program to calculate simple interest for a set of values representing principal, number of years and rate of interest.
SOL: Here also i don't know the formula to calculate simple interest so i go to chatgpt again for help. so it gave me I = PxRxT.
```
#include <stdio.h>
int main() {
    float principal, rate, time, interest;
    printf("Enter principal amount: ");
    scanf("%f", &principal);
    printf("Enter rate of interest: ");
    scanf("%f", &rate);
    printf("Enter time in years: ");
    scanf("%f", &time);
    interest = (principal * rate * time) / 100;
    printf("Simple Interest = %.2f\n", interest);
    return 0;
}

```

### CHAPTER 2
#### TYPES OF INSTRUCTIONS
1. Type declaration Instructions:

```
int a;
float b;
char c;
```
2. Arithmetic Instructions:
	   Arithmetic instructions perform mathematical operations.
	   some of the commonly used operators in C language:
	    + (Addition) 
	    - (Subtraction) 
	    * (Multiplication) 
	    / (Division) 
	    % (Modulus)
	 ![[C-20240727221507876.webp|187]]
	***Note:
	1. Operands can be int/float etc. + - * / are arithmetic operators.\
	2. % is the modular division operator 
	*  % → returns the remainder 
	* % → cannot be applied on float 
	* % → sign is same as of numerator (-5%2=-1)
	3. No operator is assumed to be present.
	4. There is no operator to perform exponentiation in C however we can use pow (x,y) from <math.h>
###### TYPE CONVERSION
An Arithmetic operation between 
• int and int → int 
• int and float → float 
• float and float → float
###### OPERATOR PRECEDENCE IN C
Have a look at the below statement: 3*x – 8*y is (3x)-(8y) or 3(x-8y)? 
In C language simple mathematical rules like BODMAS, no longer apply. 
The answer to the above questions is provided by operator precedence & associativity.

The following table lists the operator priority in C:

| PRIORITY | Operators |
| :------- | :-------- |
| 1st      | * / %     |
| 2nd      | + -       |
| 3rd      | =         |


3. Control Instructions:
	Determines the flow of control in a program four types of control instructions in C are: 
	1. Sequence Control instructions. 
	2. Decision Control instructions 
	3. Loop Control instructions 
	4. Case Control instructions.
#### CHAPTER 2 – PRACTICE SET

1. Which of the following is invalid in C? 
	a. int a=1; int b = a; 
	b. int v = 3*3; 
	c. char dt = ‘21 dec 2020’;
	SOL:  C is Wrong
2. What data type will 3.0/8 – 2 return?
	SOL: As we have learned in Athematic operations divide will execute first.
3. Write a program to check whether a number is divisible by 97 or not.
	SOL:  this can be done by:
```
#include <stdio.h>
int main() 
{
    int a,b = 97;
    printf("Enter the number: ");
    scanf("%d",&a);
    if(a%b == 0)
        printf("It is divisible by 97");
    else
        printf("It is not divisible by 97");
    return 0;
} // WE WILL LEARN ABOUT IF-ELSE IN CHAPTER 3
```
4. Explain step by step evaluation of ```3*x/y – z+k, where x=2, y=3, z=3, k=1 ```
	sol: i will let the code handle the problem instead of step by step
```
#include <stdio.h>
int main() {
    int x = 2, y = 3, z = 3, k = 1;
    int result = 3*x/y - z + k;
    printf("The result is %d\n", result);
    return 0;
}
```

### Chapter 3: CONDITION INSTRUCTIONS 
#### DECISION MAKING INSTRUCTIONS IN C
##### If–else statement
The syntax of an if-else statement in C looks like:
```
if (condition_to_be_checked) 
{ // Statements if condition is true
} else 
{ // Statements if condition is false
```
**RELATIONAL OPERATORS IN C**
Relational operators are used to evaluate conditions (true or false) inside the if statements.
Some examples of relational operators are:  ``` ==, >=, >, <, <=, !=   ```
The condition can be any valid expression. In C a non-zero value is considered to be true.
**LOGICAL OPERATORS** 
&&, || and !, are three logical operators in C. These are read as “AND”, “OR” and “NOT” They are used to provide logic to our C programs.
**USAGE OF LOGICAL OPERATORS**
1. && (AND) → is true when both the conditions are true 
	a. “1 and 0” is evaluated as false. 
	b. “0 and 0” is evaluated as false. 
	c. “1 and 1” is evaluated as true.
2. || (OR) → is true when at least one of the conditions is true. (1 or 0 → 1) (1 or 1 → 1) 
3. ! (NOT) → returns true if given false and false if given true 
	a. !(3 == 3) → evaluates to false 
	b. !(3>30) → evaluates to true.
As the number of conditions increases, the level of indentation increases. This reduces readability. Logical operators come to rescue in such cases.
**ELSE IF CLAUSE**
Instead of using multiple if statements, we can also use else if along with it thus forming an if-else if-else ladder.
```
if{ 
// Statements 
} 
else if{ // Statements 
} 
else{ // Statements 
}
```
1. Using if-else if -else reduces indents. 
2. The last “else” is optional. 
3. Also there can be any number of “else if”. 
4. Last else is executed only if all conditions fail.

| Priority |  Operator  |
| :------: | :--------: |
|    1     |     !      |
|    2     |  *, /, %   |
|    3     |    +, -    |
|    4     | <>, <=, >= |
|    5     |  == , !==  |
|    6     |     &&     |
|    7     |    \|\|    |
|    8     |     =      |
**CONDITIONAL OPERATORS**
A shorthand “if – else” can be written using the conditional or ternary operators
```
condition ? expression-if-true : expression-if-false
// Here "?" and ":" are called Ternary Operators
```
##### Switch statement
switch-case is used when we have to make a choice between number of alternatives for a given variable.
```
switch (integer expression)
{
case c1:
// code;
case c2:         // c1, c2 & c3 -> Constants 
// code;         // code -> Any valid C code. 
case c3: 
// code: 
default: 
// code; 
}
```

The value of integer-expression is matched against c1, c2, c3… If it matches any of these cases, that case along with all subsequent “case” and “default” statements are executed.

• We can use switch-case statements even by writing cases in any order of our choice (not    necessarily ascending). 
• char values are allowed as they can be easily evaluated to an integer. 
• A switch can occur within another but in practice this is rarely done.
##### ASCII VALUE:
ASCII (American Standard Code for Information Interchange) is a character encoding standard used to represent text in computers and other devices that use text. Each character is assigned a unique 7-bit code. The ASCII values for all characters range from 0 to 127.

#### CHAPTER 3 – PRACTICE SET
1) What will be the output of this program:
```
int a = 10;
if (a = 11)
	printf("I am 11");
else 
	printf("I am not 11");
```
sol: Output for this is: I am 11. 
**REASON:** Is because = is used for assignment where as == is used for equality check.

2) Write a program to determine whether a student has passed or failed. To pass, a student requires a total of 40% and at least 33% in each subject. Assume there are three subjects and take the marks as input from the user.
SOL:
```
#include <stdio.h>

int main() {
    int marks1, marks2, marks3;

    // Take marks as input from the user
    printf("Enter marks for subject 1: ");
    scanf("%d", &marks1);
    printf("Enter marks for subject 2: ");
    scanf("%d", &marks2);
    printf("Enter marks for subject 3: ");
    scanf("%d", &marks3);
    // Calculate the total marks and percentage
    int total = marks1 + marks2 + marks3;
    float percentage = total / 3.0;
    // Check if the student has passed or failed
    if(percentage >= 40 && marks1 >= 33 && marks2 >= 33 && marks3 >= 33) {
        printf("Passed\n");
    } else {
        printf("Failed\n");
    }
    return 0;
}
```

3) Write a program to determine whether a character entered by the user is lowercase or not.
SOL: To know weather the character entered is lowercase or not we need to know the concept of ASCII values and then we can solve the code.
```
#include<stdio.h>
int main()
{
	char ch = 'a';
	printf("The value of character is %d\n",ch);
	return 0;
}
```


















