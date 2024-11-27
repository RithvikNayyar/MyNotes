
YOUTUBE LINK: https://bit.ly/50HRCP, https://bit.ly/CWCWH10HR
# Basic of computing

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
![[Pasted image 20240717080151.png]]
#### Analog Computer
* They work on physical phenomena - Advantage
* They are less accurate & slow - Disadvantage
Ex: Speedometer, Voltage meter, Pressure gauge, etc. 

#### Hybrid computer
* It has some portion of digital computer & Analog Computer (ex: Digital speedometer, Digital thermometer, Electric multimeter)
___________________

![[Pasted image 20240715094407.png|541]]


__________________________________________________________________________

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

# C Programming 
### CHAPTER 1: VARIABLES, CONSTANTS & KEYWORDS
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

### CHAPTER 2: INSTRUCTIONS AND OPERATORS
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

### Chapter 4: LOOP CONTROL INSTRUCTION

**WHY LOOP:** Sometimes we want our programs to execute few sets of instructions over and over again. For example: Printing 1 to100, first 100 even numbers etc. Hence loops make it easy for a programmer to tell computer that a given set of instructions must be executed repeatedly.

**TYPES OF LOOPS:** 1. while loop 2. do-while loop 3. for loop

**WHILE LOOP:** A while loop is a control structure that executes a block of code as long as a specified condition is true. It’s essentially a repeating `if` statement. The loop ends when the condition becomes false. It’s used when the number of iterations is unknown. The condition is checked before each iteration. If the condition is false at the start, the loop body won’t execute at all.
```
int i = 0; 
while (i<10) {  // condition 
printf("the value of i is %d\n", i); 
i++; // The block keeps executing as long as the condition is true
}
```

**INCREMENT AND DECREMENT OPERATORS:** (VERY IMP TOPIC)
1. **Increment Operator (++)**:
    - Increases the value of a variable by 1.
    - Two flavors:
        - **Pre-Increment**: `++m` (Increment first, then use the value)
        - **Post-Increment**: `m++` (Use the value first, then increment)
2. **Decrement Operator (–)**:
    - Decreases the value of a variable by 1.
    - Similar flavors:
        - **Pre-Decrement**: `--m`
        - **Post-Decrement**: `m--`
* i+=2 is compound assignment which translates to i = i + 2
* Similar to += operator we have other operators like -=, *=, /=, %=

**DO-WHILE LOOP:** The syntax of do-while loop looks like this:
```
do {
//code
} while(condition);
```
The do-while loop works very similar to while loop.
* 'while' checks the condition & then executes the code.
* 'do-while' executes the code & then checks the condition.
**FOR LOOP:** the syntax of for loop looks like this:
```
for(initialize; test; increment or decrement)
{
 //code;
}
```
* Initialize --> setting a loop counter to an initial value.
* test --> Checking a condition.
* Increment --> Updating the loop counter.
**A case of decrementing for loop**
```
for(i =5; i ; i--)
	printf("%d"\n,i);
```
This for loop will keep running till it becomes 0.
The loop runs in following steps:
1. 'I' is initialized to 5
2. The condition "i"(0 or none) is tested
3. the code is executed
4. 'I' is decremented
5. Condition i is checked & code is executed if it's not 0.
**The break statement in C:** The break statement is used to exit the loop irrespective of weather the condition is true or false.
Whenever a "break" is encountered inside the loop, the control is sent outside the loop.
```
for(i=0; i<1000;i++)
{
	printf("%d",i);
	if(i==5){
		break;
	}
}
```
Output: 0 1 2 3 4 5
**The Continue Statement in C:** The continue statement is used to immediately move to the next iteration of the loop.

The control is taken to the next iteration thus skipping everything below "Continue " inside the loop for the iteration.
```
#include <studo.h>
int main() {
	int skip =5,i = 0;
	while(i<10){
		if(i == skip){
			i++;
			continue;
		}
		printf("%d\n", i);
		i++
	}
	return 0;
}
```
NOTES:
1. Sometimes. the name of the variable might not indicate the behaviour of the program.
2. Break statement completely exits the loop.
3. continue statement stops the particular iteration of the loop.

#### Chapter 4 Practice set: 
1) Write a program to print multiplication table of a given number n.
   sol: 
```
 #include<stdio.h>

int main ()
{
	 int i, n, a;
	 printf("Enter the number: ");
	 scanf("%d", &n);
	 for (i=1;i<=10;i++)
		printf("%d * %d = %d\n",n,i,n*i);
	return 0;
}  
```
2) write a program to print multiplication table of 10 in reverse order.
   sol:
```
#include<stdio.h>

int main ()
{
	 int i, n = 10;
	 for (i=10;i>=1;i--)
		printf("%d * %d = %d\n",n,i,n*i);
	return 0;
}
```


### CHAPTER 5  – FUNCTIONS AND RECURSION

Sometimes out program gets bigger and bigger in size and it's not possible for a programmer to track which piece of code is doing what.

Function is a way to break out code into chunks so that it is possible for a programmer to reuse them.

**WHAT IS A FUNCTION:** A function is a block of code which performs a particular task.
A function can be reused by the programmer in a given program any number of times.
```
#include<sudio.h>
void display();
int main(){
	int a;
	display();
	return 0;
}

void display(){
	printf("Hi i am display\n");
}
```
What does this program actually do? 
This program made a function name display, and wrote the main function, In the main function it called display function. what does it do is in between executing main function it executes display function first then executes the whole command.

**FUNCTION CALL:** A function call instructs the compiler to execute the function's body when the call is made.

**FUNCTION DEFINITION:** This part contains the exact set of instructions executed during the function call.
When a function is called from main(), the main function pauses and temporarily suspends. during this time, control transfers to the called function. once the function finishes executing, main() resumes.

* Execution of a C program starts from main()
* A C program can have more than one function
* Every function get called directly or indirectly from main().

**TYPES OF FUNCTION:** There are two types of function in C. Let's talk about them.
1.  Library functions: Commonly required functions grouped together in a library file on disk.
2. User defined function: These are the function declared and defined the user.

**WHY USE FUNCTION:** 
1. TO AVOID REWRITING THE SAME LOGIC AGAIN AND AGAIN.
2. TO KEEP TRACK OF WHAT WE ARE DOING IN A PROGRAM
3. TO TEST AND CHECK LOGIC INDEPENDENTLY 
**PASSING VALUES TO FUNCTION:** We can pass values to a function and can get a value in return from a function.
```
int sum (int a, int b)
```
A function prototype in programming is a declaration of a function that specifies its name, return type, and parameters but does not include the function body.
The above prototype means that sum is a function which takes value a and b and returns a value of type int.
Function definition of sum can be:
```
int sum(int a, int b) {
	int c;
	c = a+b;
	return c;
}
int d = sum (2,3);
```
**NOTE:** 
 1. Parameters are the values or variable placeholders in the function definition. Example a & b. 
 2. Arguments are the actual values passed to the function to make a call. Example 2 & 3. 
 3. A function can return only one value at a time. 
 4. If the passed variable is changed inside the function, the function call doesn’t change the value in the calling function.
**RECURSION:** A Function defined in C can call itself. This is called recursion. A function calling itself is also called recursive function.

Example: 
A very good example of recursion is factorial. 
Factorial(n) = 1 x 2 x 3 … x n 
Factorial(n) = 1 x 2 x3 … (n-1) x n 
Factorial(n) = Factorial (n-1) x n 
Since we can write factorial of a number in terms of itself, we can program it using recursion.
```
int factorial(int x) {
int f; 
if (x == 0 || x == 1) { 
	return 1; // a program to calculate factorial using recursion 
} else { 
	f = x * factorial(x - 1); 
	return f; 
	} 
}
```

**DRY RUN OF RECURSIVE FACTORIAL PROGRAM:** 
![[C-20240803190753725.webp|200]]
note:
1. Recursion is often a direct way to implement certain algorithms, but not always the most direct for every algorithm. Recursion is particularly suited for problems that can be divided into smaller, similar subproblems (like factorial computation or tree traversal), but for some algorithms, iterative approaches might be more straightforward or efficient. 
2. The condition in a recursive function that stops further recursion is called the base case. This correction clarifies that the base case is crucial as it prevents infinite recursion and ensures the function terminates correctly. 
3. Sometimes, due to an oversight by the programmer, a recursive function can continue to run indefinitely without reaching a base case, potentially causing a stack overflow or memory error. This statement highlights the risk of infinite recursion and its consequences, emphasizing the importance of properly defining base cases in recursive functions.

#### CHAPTER 5 - PRACTICE SET
1. Write a program using function to find average of three numbers.
sol: 
```
#include <stdio.h>

// Function to calculate the average of three numbers
float findAverage(float num1, float num2, float num3) {
    return (num1 + num2 + num3) / 3;
}

int main() {
    float a, b, c, average;

    // Input three numbers
    printf("Enter three numbers: ");
    scanf("%f %f %f", &a, &b, &c);

    // Calculate the average
    average = findAverage(a, b, c);

    // Output the result
    printf("The average of %.2f, %.2f, and %.2f is %.2f\n", a, b, c, average);

    return 0;
}

```
2. Write a function to convert Celsius temperature into Fahrenheit.
sol:
```
#include <stdio.h>

// Function to convert Celsius to Fahrenheit
float celsiusToFahrenheit(float celsius) {
    return (celsius * 9/5) + 32;
}

int main() {
    float celsius, fahrenheit;

    // Input temperature in Celsius
    printf("Enter temperature in Celsius: ");
    scanf("%f", &celsius);

    // Convert to Fahrenheit
    fahrenheit = celsiusToFahrenheit(celsius);

    // Output the result
    printf("%.2f Celsius is %.2f Fahrenheit\n", celsius, fahrenheit);

    return 0;
}

```
3. Write a function to calculate force of attraction on a body of mass ‘m’ exerted by earth. Consider g = 9.8m/s2.
sol: 
```
#include <stdio.h>

// Function to calculate the force of attraction
float calculateForce(float mass) {
    const float g = 9.8;  // Gravitational constant
    return mass * g;
}

int main() {
    float mass, force;

    // Input mass of the body
    printf("Enter the mass of the body (in kg): ");
    scanf("%f", &mass);

    // Calculate the force of attraction
    force = calculateForce(mass);

    // Output the result
    printf("The force of attraction on a body of mass %.2f kg is %.2f N\n", mass, force);

    return 0;
}

```

4. Write a program using recursion to calculate nth element of Fibonacci series.
sol:
```
#include <stdio.h>

// Function to calculate the nth Fibonacci number using recursion
int fibonacci(int n) {
    if (n <= 1) {
        return n;  // Base cases: fibonacci(0) = 0, fibonacci(1) = 1
    } else {
        return fibonacci(n - 1) + fibonacci(n - 2);  // Recursive case
    }
}

int main() {
    int n;

    // Input the position in the Fibonacci series
    printf("Enter the position in the Fibonacci series: ");
    scanf("%d", &n);

    // Calculate the nth Fibonacci number
    int result = fibonacci(n);

    // Output the result
    printf("The %dth Fibonacci number is %d\n", n, result);

    return 0;
}

```
5. Write a recursive function to calculate the sum of first ‘n’ natural numbers.
sol:
```
#include <stdio.h>

// Recursive function to calculate the sum of first n natural numbers
int sumOfNaturalNumbers(int n) {
    if (n == 0) {
        return 0;  // Base case
    } else {
        return n + sumOfNaturalNumbers(n - 1);  // Recursive case
    }
}

int main() {
    int n;

    // Input the value of n
    printf("Enter a positive integer: ");
    scanf("%d", &n);

    // Calculate the sum of first n natural numbers
    int sum = sumOfNaturalNumbers(n);

    // Output the result
    printf("The sum of the first %d natural numbers is %d\n", n, sum);

    return 0;
}

```

6. Write a program using function to print the following pattern (first n lines) 
```
*
* * *
* * * * *
```
sol:
```
#include <stdio.h>

// Function to print the pattern
void printPattern(int n) {
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= (2 * i - 1); j++) {
            printf("* ");
        }
        printf("\n");
    }
}

int main() {
    int n;

    // Input the number of lines
    printf("Enter the number of lines: ");
    scanf("%d", &n);

    // Print the pattern
    printPattern(n);

    return 0;
}
```

### CHAPTER 6 - POINTERS
A pointer is a variable which stores the address of another variable.
![[C-20240803195452608.webp|459]]

**THE “ADDRESS OF” (&) OPERATOR:** The address of operator is used to obtain the address of a given variable.
If you refer to the diagrams above, 
&i → 87994 
&j → 87998 
Format specifier for printing pointer address is ‘%p’.

**THE VALUE AT ADDRESS OPERATOR( * ):** The value at address or * operator is used to obtain the value present at a given memory address. It is denoted by *.
 * * (&i) =72 
 * * (&j) = 87994
 **HOW TO DECLARE A POINTER?** A pointer is declared using the following syntax.
 * int * j => declare a variable j of type int - pointer
 * j = &i => store address of i in j.
Just like pointer of type integer, we also have pointers to char, float etc.
```
int* ptr;
float* ptr;
char* ptr;
```
Although it's a good practice to use meaningful variable names, we should be very careful while reading and working on programs from fellow programmers.
**A PROGRAM TO DEMONSTRATE POINTERS**
```
#include<stdio.h>
int main(){
	int i =8;
	int* j;
	j = &i;
	printf("add i = %u\n,&i");
	printf("add i = %u\n,j");
	printf("add j = %u\n,&j");
	printf("value i= %d\n",i);
	printf("value i= %d\n",*(&i)); 
	printf("value i= %d\n",*j);
	return 0;
}
```
OUTPUT:
```
add i= 87994 
add i= 87994 
add j= 87998 
value i= 8 
value i= 8 
value i= 8
```
This program sums it all. If you understand it, you have got the idea of pointers.
**POINTER TO A POINTER:** Just like ‘j’ is pointing to ‘i’ or storing the address of ‘i’, we can have another variable k which can further store the address of ‘j’. What will be the type of ‘k’?
```
int **k; 
k = &j;
```
![[C-20240805135216381.webp|293]]
36 We can even go further one level and create a variable ‘l’ of type int*** to store the address of ‘k’. We mostly use int* and int** sometimes in real world programs.
**TYPES OF FUNCTION CALL:** Based on the way we pass arguments to the function, function calls are of two types. 
1. Call by value → Sending the values of arguments. 
2. Call by reference → Sending the address of arguments.

**CALL BY VALUE:** Here the values of the arguments are passed to the function. Consider this example:
```
int c = sum (3,4); //assume x=3 and y=4
```
If sum is defined as sum (int a, int b), the values 3 and 4 are copied to a and b. Now even if we change a and b, nothing happens to the variables x and y. 
This is call by value. In C we usually make a call by value.

**CALL BY REFERENCE:** Here the address of the variables is passed to the function as arguments. 
Now since the addresses are passed to the function, the function can now modify the value of a variable in calling function using * and & operators.
```
void swap (int *x, int *y) { 
	int temp; 
	temp = *x; 
	*x = *y; 
	*y = temp; 
}
```
This function is capable of swapping the values passed to it. If a = 3 and b = 4 before a call to swap(a, b), then a = 4 and b = 3 after calling swap.
```
int main(){ 
	int a = 3; 
	int b = 4; // a is 3 and b is 4 
	swap(&a, &b); 
	return 0; //now a is 4 and b is 3 }
```

#### CHAPTER 6 - PRACTICE SET

### CHAPTER 7 - ARRAYS
An array is a collection of similar elements. Array allows a single variable to store multiple values.
**SYNTAX:** 
```
int marks[90]; // integer array 
char name[20]; // character array or string 
float percentile[90]; // float array
```
The values can now be assigned to make array like this:
```
marks[0] = 33; 
marks[1] = 12;
```
Note: It is very important to note that the array index starts with 0.
![[C-20240805140327083.webp|284]]
**ACCESSING ELEMENTS:** Elements of an array can be accessed using:
```
scanf("%d", &marks[0]); // input first value
printf("%d", marks[0]); // output first value of the array
```
**INITIALIZATION OF AN ARRAY:** There are many other ways in which an array can be initialized.
```
int cgpa[3] = {9, 8, 8}; // arrays can be initialized while declaration float marks[] = {33, 40};
```
**ARRAYS IN MEMORY:** Consider this array:
```
int arr[3] = {1, 2, 3} // 1 integer = 4 bytes
```
This will reserve 4 x 3 = 12 bytes in memory (4 bytes for each integer).
![[C-20240805140651528.webp|289]]
**POINTER ARITHMETIC:** 
A pointer can be incremented to point to the next memory location of that type. Consider this example:
```
int i = 32; 
int *a = &i; // a = 87994 
a++; // address of i or value of a = 87998 
char a = 'A'; 
char *b = &a; // a= 87994 
b++; // now a = 87995 

float i = 1.7; 
float *a = &i; // now a = 87994 
a++; // now a = 87998
```
Following operations can be performed on a pointer: 
1. Addition of a number to a pointer. 
2. Subtraction of a number from a pointer. 
3. Subtraction of one pointer from another. 
4. Comparison of two pointer variables.
**ACCESSING ARRAY USING POINTERS:** Consider this array:
![[C-20240805140857836.webp|186]]
If ptr points to index 0, ptr++ will point to index 1 & so on… 
This way we can have an integer pointer pointing to first element of the array like this:
```
int *ptr = &arr[0]; // or simple arr 
ptr++; 
*ptr // will have 9 as its value
```
**PASSING ARRAY TO FUNCTIONS:** Array can be passed to the functions like this:
```
printArray(arr, n); // function call 
void printArray(int *i, int n); // function prototype 
// or 
void printArray(int i[], int n);
```
**MULTIDIMENSIONAL ARRAYS:** An array can be of 2 dimension/ 3 dimension/ n dimensions. 
A 2 dimensions array can be defined like this:
```
int arr[3][2] = {{1, 4} {7, 9} {11, 22}};
// We can access the elements of this array as arr[0][0] , arr[0][1] & so on …
```
**2-D ARRAYS IN MEMORY:** 
A 2d array like a 1d array is stored in contiguous memory blocks like this:
![[C-20240805141509830.webp|319]]
#### CHAPTER 7 – PRACTICE SET

### CHAPTER 8 – STRINGS
A string is a 1-D character array terminated by a null character (‘\0’) 
A null character is used to denote the termination of a string. Characters are stored in contiguous memory locations.






