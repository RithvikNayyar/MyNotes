
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
![[Pasted image 20240715094151.png]] 

#### Analog Computer
* They work on physical phenomena - Advantage
* They are less accurate & slow - Disadvantage
Ex: Speedometer, Voltage meter, Pressure gauge, etc. 

#### Hybrid computer
* It has some portion of digital computer & Analog Computer (ex: Digital speedometer, Digital thermometer, Electric multimeter)
__________________________________________________________________________
![[Pasted image 20240715094407.png]]
![[Pasted image 20240715094454.png]]
![[Pasted image 20240715100243.png]]
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
![[Pasted image 20240715105723.png]]

#### Software & It's Development
* Software either control hardware or do some specific task
* Software is a set of instructions written in specific computer understandable form to perform specific task.
* EX: When you are on a desktop and type something like your name but nothing happens and then you open a notepad and type your name then you see your name on the notepad. So this show that I/O devices are controlled through software.
![[Pasted image 20240715111547.png]] 

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
![[Pasted image 20240716070523.png]]

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
![[Pasted image 20240716071718.png]]

##### Compiler & Interpreter
- A translator or programming language processor is a generic term that can refer to anything that converts code from one computer language into another.
- Compiler and interpreter are translator for high level Language.
![[Pasted image 20240716073124.png]]

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
![[Pasted image 20240716084721.png]]
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
![[Pasted image 20240717080151.png|277]]

#### How to write C Program
##### Rules for making C
1. C is a functional programming language. (Function is a set of statement which perform some action)
![[Pasted image 20240717082009.png|652]]
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
![[Pasted image 20240717100150.png]]
![[Pasted image 20240717101015.png|459]] 

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
![[C all in 1 notes-20240717102323564.webp]]

#### COMMENTS

// 












