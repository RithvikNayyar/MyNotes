#### The History of JAVA
 
 **The Genesis: The Green Project (1991):**
 
- **The Team:** Initiated by a small team at **Sun Microsystems** known as the "Green Team," led by **James Gosling**, Mike Sheridan, and Patrick Naughton.
- **The Goal:** To develop a technology for programming next-generation smart consumer electronics (like interactive televisions, set-top boxes, and appliances).
- **The Problem:** Existing languages like C and C++ were platform-dependent (compiled for a specific hardware architecture) and prone to errors (memory leaks, pointer arithmetic). Consumer electronics used widely varying chips.
- **The Solution:** Gosling began developing a new language with a virtual machine concept. The code would compile into an intermediate state (bytecode) that a platform-specific software (the JVM) could read, making the language platform-independent.
- **Original Name:** Gosling initially named it **"Greentalk"** (with file extension `.gt`), which later became **"Oak"**, named after an oak tree outside his office window.
![[image.png]]

**The Pivot and the Naming (1992 - 1994):**

- **1992:** The Green Team demonstrated their system with an interactive, handheld home-entertainment controller called the **"Star 7" (*7)**. It featured an animated mascot named "Duke," who remains Java's mascot today.
- **1993:** The interactive TV industry was not yet ready for this advanced technology. However, the World Wide Web was just beginning to explode in popularity.
- **The Shift:** The team realized their platform-independent, secure, and robust language was perfect for web browsers. They pivoted from consumer electronics to the Internet.
- **1994:** The name "Oak" was already trademarked by Oak Technologies. The team had a brainstorming session and chose **"Java"** (named after Java coffee from Indonesia). They also built **WebRunner** (later renamed **HotJava**), the first web browser capable of running Java "applets" (small Java programs running inside the browser).

**Public Release and Rapid Adoption (1995 - 1996):** 

- **May 23, 1995:** Sun Microsystems officially released the first public beta of Java (Java 1.0 a 2).
- **The Catchphrase:** Java was marketed with the famous slogan: **"Write Once, Run Anywhere" (WORA)**.
- **Netscape Partnership:** Marc Andreessen of Netscape (the dominant web browser at the time) announced they would incorporate Java support into Netscape Navigator. This catapulted Java into mainstream popularity.
- **January 1996:** The first stable version, **JDK 1.0** (Java Development Kit), was released.    
- **Key Design Principles:** Sun defined Java as: Simple, Object-Oriented, Network-Savvy, Robust, Secure, Architecture-Neutral, Portable, High-Performance, Multithreaded, and Dynamic.

**The Golden Era of Growth: J2SE (1997 - 2008):**
Java evolved rapidly through major version releases, adding core features that defined modern enterprise software.
- **JDK 1.1 (1997):** Introduced major additions like Inner Classes, JavaBeans, JDBC (Java Database Connectivity), and RMI (Remote Method Invocation).
- **J2SE 1.2 (1998):** A massive milestone. Sun rebranded it as "Java 2" (J2SE - Java 2 Platform, Standard Edition). Introduced the **Collections Framework** and the **Swing** GUI toolkit.
- **J2SE 1.3 (2000) & 1.4 (2002):** Focused on performance improvements (HotSpot JVM), regular expressions, and XML parsing.
- **J2SE 5.0 (2004):** One of the most significant updates in Java's history. It introduced:
    - **Generics:** Providing compile-time type safety.
    - **Annotations:** Metadata for code.
    - **Autoboxing/Unboxing:** Automatic conversion between primitives and their object wrappers.
    - **Enums:** Type-safe enumerations.
    - **Varargs:** Variable-length arguments.
- **Java SE 6 (2006):** Rebranded simply to "Java SE 6". Dropped the "J2" naming convention.

**The Oracle Era and Modern Java (2009 - Present):**
- **2009-2010:** **Oracle Corporation acquired Sun Microsystems**, taking ownership of Java. This caused some initial friction in the open-source community, leading to the creation of independent forks (though OpenJDK remains the official open-source reference implementation).
- **Java SE 7 (2011):** The first release under Oracle. Introduced the `try-with-resources` statement and the diamond operator `<>`.
- **Java SE 8 (2014):** Another massive paradigm shift. It introduced functional programming concepts to Java, specifically:
    - **Lambda Expressions:** Enabling functional-style operations.
    - **Streams API:** For processing collections of objects.
    - **New Date/Time API.**
- **Java SE 9 (2017):** Introduced **Project Jigsaw** (the Java Module System) to modularize the JDK itself, making it lighter and faster.
- **The New Release Cycle (2018 onward):** Oracle changed Java's release cadence from feature-driven (releasing every few years) to time-driven, releasing a new feature update **every 6 months** (March and September).
- **LTS (Long-Term Support) Versions:** Because updating every 6 months is hard for enterprises, Oracle designates specific versions for Long-Term Support (initially every 3 years, now every 2 years).
    - Major LTS versions include: **Java 8, Java 11, Java 17, Java 21 and Java 25**.

##### Problems with Existing languages (90's):

1. Platform Dependency (The Biggest Hurdle):
- **The Problem:** C and C++ are **compiled languages** that translate source code directly into native machine code (binary consisting of 0's and 1's) specific to a particular hardware architecture and operating system.
- **The Impact:** If you wrote and compiled a C++ program for a Windows machine with an Intel processor, that compiled file would be complete gibberish to a Mac using a Motorola processor, or a set-top box using an ARM chip.
- **Why it mattered:** To run software on different machines, developers had to rewrite parts of the code and recompile it for _every single target platform_. This made distributing software across diverse hardware (like early smart devices or internet users) an expensive, logistical nightmare.

2. Manual Memory Management

- **The Problem:** In C and C++, the programmer is entirely responsible for allocating and freeing up memory using functions like `malloc()`, `calloc()`, `free()` (in C) or `new` and `delete` (in C++).
- **The Impact:** Humans make mistakes. This manual process frequently led to two major, difficult-to-debug issues:
    - **Memory Leaks:** A developer allocates memory for an object but forgets to free it when it is no longer needed. The program slowly eats up all available RAM until it crashes.
    - **Dangling Pointers:** A developer frees memory but accidentally leaves a pointer aiming at that now-empty address. If the program tries to use that pointer later, it causes a severe crash (segmentation fault).

3. The Danger of Explicit Pointers
- **The Problem:** C and C++ rely heavily on pointers, variables that store the direct, physical memory address of another value.
- **The Impact:** While pointers grant developers immense power and speed to manipulate memory directly, they are notoriously easy to misuse. A slight miscalculation in "pointer arithmetic" can result in a program accidentally overwriting crucial system memory or completely unrelated data.

4. Severe Security Vulnerabilities
- **The Problem:** Because C and C++ allow direct memory access via pointers and lack built-in "bounds checking" (verifying that you aren't trying to stuff more data into an array than it can hold), they are highly vulnerable to exploitation.
- **The Impact:** Malicious actors could use techniques like **Buffer Overflows** to overwrite memory and inject malicious code.
- **Why it mattered:** As the World Wide Web emerged, the idea of downloading and running a C/C++ program from an unknown server was considered incredibly dangerous. There was no "sandbox" to contain the code.

5. Lack of Native Multithreading:
- **The Problem:** C and C++ did not have built-in, standardized support for multithreading (running multiple tasks concurrently within the same program) at the language level.
- **The Impact:** Developers had to rely on operating system-specific APIs (like Windows Threads or POSIX pthreads for Unix). This meant threading code written for Windows had to be completely rewritten for Linux, further hurting portability.

6. Extreme Complexity
- **The Problem:** C++ was designed as an extension of C, adding Object-Oriented features while maintaining backward compatibility. Over time, it became a massive, complex language.
- **The Impact:** Features like **Multiple Inheritance** (a class inheriting from multiple parent classes) often led to convoluted class hierarchies and the infamous "Diamond Problem" (ambiguity in which parent's method to use). Concepts like **Operator Overloading** (changing what basic math symbols do) made code hard to read and maintain for new developers.

#### **How Java solved this problem:**
- **Platform Independence:** Introduced bytecode and the **JVM** (Java Virtual Machine) to achieve "Write Once, Run Anywhere" (WORA), replacing OS-specific compilation.
- **Automatic Memory Management:** Replaced manual memory allocation with the **Garbage Collector**, an automated background process that eliminates memory leaks.
- **No Explicit Pointers:** Removed direct memory manipulation, preventing memory corruption and fatal pointer errors.
- **Enhanced Security:** Code executes inside the secure JVM "sandbox" with strict array bounds checking, preventing malicious attacks like buffer overflows.
- **Simplified Language:** Removed complex, error-prone C++ features like multiple class inheritance and operator overloading to make code easier to read and maintain.
- **Built-in Multithreading:** Added native, OS-independent multithreading directly into the language, rather than relying on different operating system APIs.


Java uses a two-step process—compilation and interpretation—to achieve platform independence.
- **Step 1: Source Code:** You write human-readable Java code and save it with a `.java` extension.
- **Step 2: Compilation (`javac`):** The Java Compiler does _not_ translate this code into machine code. Instead, it translates it into an intermediate, platform-neutral format called **Bytecode**. This creates a `.class` file.
- **Step 3: The JVM Takes Over:** You move that `.class` file to any device. The Java Virtual Machine (JVM) installed on that specific device reads the bytecode.
- **Step 4: Execution:** The JVM translates the bytecode into the native machine code (0's and 1's) that the specific hardware and operating system can understand and execute.
![[image 2.png]]

#### Working of Java & JVM:
The JVM's job is to take that compiled Bytecode and actually run it on your machine. To do this efficiently, the JVM acts as a "hybrid" system inside its Execution Engine, using both an **Interpreter** and a **Just-In-Time (JIT) Compiler**.

<b><u>The Step-by-Step JVM Execution Process</u></b>
**1. Bytecode is Loaded:** The JVM's Class Loader subsystem brings the Bytecode into the computer's memory so the Execution Engine can access it.

**2. The Interpreter Takes the Lead:** The Execution Engine's **Interpreter** starts first. It reads the Bytecode line-by-line, translates each instruction into hardware-specific machine code (0's and 1's), and executes it immediately.
- _Advantage:_ The program starts running instantly without waiting for a massive compilation process.
- _Disadvantage:_ It is slow. If you have a loop that runs 10,000 times, the interpreter stubbornly translates the exact same lines of code 10,000 times.

**3. The JIT Compiler Monitors (The Profiler):** While the Interpreter is working, the **Just-In-Time (JIT) Compiler** quietly watches in the background using a component called the Profiler. It counts how many times each method or block of code is called to identify **"hotspots"** (code that is executed repeatedly).

**4. JIT Compilation is Triggered:** When the Profiler decides a specific block of code is a "hotspot" (e.g., that loop running 10,000 times), the JIT Compiler steps in. It takes that _entire block_ of Bytecode and compiles it directly into native machine code all at once.

**5. Optimization and Storage:** The JIT Compiler doesn't just translate the code; it optimizes it to run as fast as possible on your specific CPU. It then stores this highly optimized, native machine code in a special memory area called the **Code Cache**.

**6. Direct Execution (The Speed Boost):** The next time the program needs to run that specific block of code, the JVM bypasses the slow Interpreter entirely. Instead, it grabs the pre-compiled, optimized machine code directly from the Code Cache and executes it instantly.
![[image 4.png]]
> Java uses a hybrid approach. The **Interpreter** provides a fast startup time by reading code line-by-line, while the **JIT Compiler** steps in to compile heavily used "hotspots" into pure machine code, giving Java the blazing fast performance of a fully compiled language over time.

• JDK (Java Development Kit): The full SDK for developers. Includes JRE + compiler (`javac`) + debuggers.
• JRE (Java Runtime Environment): The software layer needed to run Java apps. Includes JVM + libraries. (Note: Included in JDK).
• JSE (Java Standard Edition): The core Java platform. Used for desktop apps and basic API libraries.
• JEE (Java Enterprise Edition): Built on top of JSE. Used for large-scale, multi-tier enterprise apps (servers, web services).
• JME (Java Micro Edition): A subset of JSE for resource-constrained devices like embedded systems and old mobile phones.

#### **Core Concepts of Java**

##### **Variables in Java:** 
- A variable is a name memory location (a container) used to store data while a java program is running.
- Java is strongly, statically types language. That means every variable must be declared with a specific data type before it can be used.
**Declaration and initialization**
Creating a variable happens in two steps (which can be combined):
- **Declaration**: Telling the JVM the variable's type and name
  - `int age:`
- **Initialization:** Assigning a value to that variable for the first time using the assignment operator (`=`).
  - `age = 25;`
- **Combined (Most common):** `int age = 25;` 
![[image 1.png|634]]
> We will learn about this later

**Rules for Naming Variables (Identifiers)**
Java has strict rules and widely accepted conventions for naming variables:
**The Rules (Compiler will throw an error if broken):**
- Must begin with a letter (A-Z or a-z), a dollar sign ( `$` ), or an underscore ( `_` ). _Note: It is best practice to avoid starting with `$` or `_` ._
- Cannot start with a number.
- Cannot contain spaces.
- Cannot be a reserved Java keyword (like `class` , `public` , `int` , `static` ).
- **Case-Sensitive:** `myAge` and `myage` are considered two completely different variables.
**The Convention (Industry standard best practice):**
- Use **camelCase**: Start with a lowercase letter, and capitalize the first letter of each subsequent word (e.g., `bankAccountNumber` , `firstName` ).


##### **Data Types in Java**

Because Java is a **strongly typed** language, every variable must have a designated data type before it can be used. The data type tells the compiler two important things:
1. What _kind_ of data the variable can hold (numbers, text, true/false).
2. Exactly how much _memory_ to allocate for it.

In Java, data types are divided into two primary categories: **Primitive** and **Non-Primitive**

1. Primitive Data Types (The Core 8)
- Primitive data types are the most basic data types available in Java. They are built directly into the language, hold simple values directly in memory (the Stack), and have a fixed, predefined memory size.
There are exactly **8 primitive data types**, grouped into four categories:
![[image 5.png]]
