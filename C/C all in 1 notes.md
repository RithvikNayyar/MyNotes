
YOUTUBE LINK: https://bit.ly/50HRCP 
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


























