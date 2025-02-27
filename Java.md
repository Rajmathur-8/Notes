## Introduction to Java
Java is a **class-based, object-oriented** programming language designed to be simple, secure, and platform-independent. It was created by **James Gosling** at **Sun Microsystems** in **1995**.

---

## Key Features of Java

### 1. Platform Independence (Write Once, Run Anywhere - WORA)
Java programs are **compiled** into **bytecode** instead of machine code, allowing execution on any system with a **Java Virtual Machine (JVM)**.

```java
public class Example {
    public static void main(String[] args) {
        System.out.println("This will run on any system with JVM!");
    }
}
```

---

### 2. Object-Oriented Programming (OOP)
Java follows **OOP principles**:
- **Abstraction** - Hiding complex details
- **Encapsulation** - Wrapping data and methods inside a class
- **Inheritance** - One class acquires properties of another
- **Polymorphism** - Methods behave differently based on objects

```java
class Animal {
    void sound() {
        System.out.println("Animals make sound");
    }
}
class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks");
    }
}
public class Example {
    public static void main(String args[]) {
        Animal a = new Dog();  
        a.sound(); // Output: Dog barks
    }
}  
```

---

### 3. Simplicity
Java is simpler than C++ because it:
- **Does not use pointers**
- **Has automatic memory management**
- **Removes complex features like operator overloading**

```java
int number = 10;
System.out.println("Number is: " + number);
```

---

### 4. Robustness (Reliability)
Java detects errors **at compile-time** and **runtime** and supports **exception handling**.

```java
public class Example {
    public static void main(String[] args) {
        try {
            int result = 10 / 0;
        } catch (ArithmeticException e) {
            System.out.println("Cannot divide by zero!");
        }
    }
}
```

---

### 5. Security
Java is secure because it **does not use pointers** and **runs programs in a JVM sandbox**.

```java
int[] arr = new int[5];
arr[6] = 10;  // Throws ArrayIndexOutOfBoundsException
```

---

### 6. Multithreading
Java supports **multithreading** for executing multiple tasks simultaneously.

```java
class MyThread extends Thread {
    public void run() {
        System.out.println("Thread is running...");
    }
}
public class Example {
    public static void main(String args[]) {
        MyThread t1 = new MyThread();
        t1.start();
    }
}
```

---

### 7. High Performance
Java is **faster than interpreted languages** due to the **Just-In-Time (JIT) compiler**, which converts **bytecode to machine code at runtime**.

---

## How Java Code Executes?
### **Step 1: Writing the Program**
Write Java code in an IDE or text editor and save it with a `.java` extension.

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### **Step 2: Compiling the Program**
Run the command:
```
javac HelloWorld.java
```

### **Step 3: Running the Program**
Run the command:
```
java HelloWorld
```

---

## Java Terminologies
- **JVM (Java Virtual Machine)** - Executes Java bytecode
- **Bytecode** - Platform-independent intermediate code
- **JDK (Java Development Kit)** - Includes `javac`, JVM, and libraries
- **JRE (Java Runtime Environment)** - Includes JVM + libraries for running Java programs
- **Garbage Collector** - Automatically manages memory

---

## Advantages of Java
✅ **Platform-independent** – Runs on any system with a JVM  
✅ **Object-Oriented** – Modular and reusable code  
✅ **Secure** – No direct memory access (unlike C/C++)  
✅ **Automatic Memory Management** – No manual allocation/deallocation  
✅ **Large Community Support** – Millions of developers worldwide  

---

## Disadvantages of Java
❌ **Slower than C/C++** – Runs on JVM instead of directly on hardware  
❌ **Memory Consumption** – Uses more memory due to garbage collection  

---

## Conclusion
Java is a powerful, versatile language used for **web apps, mobile apps, games, and enterprise software**. 
Understanding **OOP, JVM, and Java fundamentals** will help you build efficient applications.  

---
# Java vs C++: A Comparative Analysis

Nowadays, Java and C++ are widely used in competitive programming and industry applications. Both languages offer unique advantages that make them popular among developers.

## Similarities between Java and C++

### 1. Execution
- **Java:** At compile-time, Java source code (`.java` file) is converted into bytecode (`.class` file). The JVM (Java Virtual Machine) loads the `.class` file and converts it to machine code using an interpreter and the Just-In-Time (JIT) compiler.
- **C++:** Uses a compiler to directly convert the source code into machine code. C++ is faster than Java but is not platform-independent.

### 2. Features Comparison
Even though both languages use Object-Oriented Programming (OOP) concepts, neither can be termed 100% object-oriented.

| Feature              | C++  | Java |
|----------------------|------|------|
| Abstraction         | Yes  | Yes  |
| Encapsulation       | Yes  | Yes  |
| Single Inheritance  | Yes  | Yes  |
| Multiple Inheritance| Yes  | No   |
| Polymorphism        | Yes  | Yes  |
| Static Binding      | Yes  | Yes  |
| Dynamic Binding     | Yes  | Yes  |
| Operator Overloading| Yes  | No   |
| Header Files        | Yes  | No   |
| Pointers            | Yes  | No   |
| Global Variables    | Yes  | No   |
| Template Class      | Yes  | No   |
| Interfaces & Packages | No  | Yes  |
| API                 | No   | Yes  |

## Syntax Differences

### C++ Example
```cpp
#include <iostream>
using namespace std;
 
int main() {
    cout << "GFG!";
    return 0;
}
```

### Java Example
```java
/*package whatever // do not write package name here */
 
import java.io.*;
 
class GFG {
    public static void main (String[] args) {
        System.out.println("GFG!");
    }
}
```

## Applications of Java vs C++

### Applications of C++
- Developing large software (e.g., passenger reservation systems)
- MySQL database is written in C++
- Game Development (for fast execution)
- Google Chromium browser, file system, and cluster data processing
- Adobe Premiere, Photoshop, and Illustrator
- Real-time physical simulations, high-performance image processing
- Advanced medical equipment (e.g., MRI machines)

### Applications of Java
- Desktop GUI Applications
- Android and Mobile application development
- Embedded technologies (SIM cards, disk players, TV, etc.)
- Java EE for enterprise software
- Web application development

## Key Differences Between Java and C++

| Sl. No. | Parameter                    | Java                                      | C++                                      |
|---------|------------------------------|------------------------------------------|------------------------------------------|
| 1       | Founder                      | James Gosling (Sun Microsystems)         | Bjarne Stroustrup (Bell Labs, 1979)      |
| 2       | First Release                | May 23, 1995                             | October 1985                             |
| 3       | Stable Release               | Java SE 18 (March 22, 2022)              | C++20 (December 15, 2020)               |
| 4       | Official Website             | [oracle.com/java](https://oracle.com/java) | [isocpp.org](https://isocpp.org)        |
| 5       | Influenced By                | Ada 83, Pascal, C++, C#, etc.            | Ada, ALGOL 68, C, Simula, Smalltalk, etc. |
| 6       | Influenced To                | C#, Kotlin, PHP, Python, Scala, etc.     | Java, Perl, Python, Rust, etc.          |
| 7       | Platform Dependency          | Platform-independent                     | Platform-dependent                       |
| 8       | Portability                  | Portable                                 | Not portable                             |
| 9       | Compilation                  | Compiled and Interpreted                 | Compiled                                 |
| 10      | Memory Management            | System-controlled                        | Manual                                   |
| 11      | Virtual Keyword              | No                                       | Yes                                      |
| 12      | Multiple Inheritance         | No (uses interfaces)                     | Yes                                      |
| 13      | Overloading                  | Method overloading only                  | Method and operator overloading         |
| 14      | Pointers                     | Limited support                          | Strong support                           |
| 15      | Libraries                     | Java Native Interfaces                   | Direct system library calls             |
| 16      | Documentation Comments       | Supported (`/** .. */`)                  | Not supported                            |
| 17      | Thread Support               | Built-in multithreading                  | Requires third-party libraries          |
| 18      | Type                         | Object-Oriented                          | Procedural + Object-Oriented            |
| 19      | I/O Mechanism                | System.in & System.out                   | `cin` & `cout`                          |
| 20      | goto Keyword                 | Not Supported                            | Supported                                |
| 21      | Structures & Unions          | Not Supported                            | Supported                                |
| 22      | Parameter Passing            | Pass by Value                            | Pass by Value & Reference               |
| 23      | Inheritance Tree             | Single inheritance tree                  | Fresh inheritance tree always created   |
| 24      | Global Scope                 | No global scope                          | Supports global & namespace scope       |
| 25      | Object Management            | Automatic (garbage collection)           | Manual (`new` & `delete`)               |
| 26      | Call by Value & Reference    | Only call by value                       | Call by value & call by reference       |
| 27      | Hardware Interaction         | Less interactive                         | More interactive                         |
| 28      | Primary Uses                 | Web, Mobile, Enterprise, Cloud, IoT      | Game Engines, OS, Browsers, VR, DBMS    |
| 29      | Applications Built           | Wikipedia, LinkedIn, Uber, Minecraft     | Mozilla Firefox, Amazon, Spotify        |

## Conclusion
Both Java and C++ are powerful programming languages with their unique strengths. Java is more suited for platform-independent and enterprise applications, whereas C++ is preferable for system programming and high-performance applications.
---
# Java Syntax and Structure

Java is an object-oriented programming language known for its simplicity, portability, and robustness. Its syntax is closely aligned with C and C++, making it easier to understand.

## Structure of a Java Program
A basic Java program consists of several components that create a functional application. Here is an example:

```java
// FileName : "Example.java".

public class Example {
    // The main method is the entry point of a Java Program
    public static void main(String[] args) {
        // Prints "Hello, Java!" to the console
        System.out.println("Hello, Java!");
    }
}
```

### Output:
```
Hello, Java!
```

### Explanation:
1. **Class Declaration:** Every Java program starts with a class declaration using the `class` keyword.
2. **Object:** Objects are instances of a class.
3. **Main Method:** `public static void main(String[] args)` is the entry point of execution.
4. **Statements:** Each line of code inside the method must end with a semicolon `;`.

## Steps to Compile and Run a Java Program

1. Compile the Java Program:
   ```sh
   javac Example.java
   ```
2. Execute the compiled bytecode:
   ```sh
   java Example
   ```

## Java Syntax Key Elements

### 1. Comments in Java
There are three types of comments in Java:

#### Single-line Comment:
```java
// This is a single-line comment
```

#### Multi-line Comment:
```java
/* This is
   a multi-line comment */
```

#### Documentation Comment:
```java
/**
 * This is a doc comment
 */
```

### 2. Source File Naming Rules

#### With a public class:
```java
public class MyClass {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
**File Name:** `MyClass.java` (Must match public class name)

#### Without a public class:
```java
class Test {
    public static void main(String[] args) {
        System.out.println("Hello, Java!");
    }
}
```
**File Name:** Can be `Test.java`, `Example.java`, or any name.

### 3. Case Sensitivity
Java is case-sensitive:

```java
System.out.println("Valid Syntax"); // Correct
system.out.println("Invalid Syntax"); // Incorrect (System should be capitalized)
```

### 4. Class Naming Rules
- First letter should be uppercase.
- No special characters except `_` and `$` (though discouraged).

```java
class MyJavaProgram {}  // Valid
class 1Program {}       // Invalid
class $MyProgram {}     // Valid but discouraged
```

### 5. Method Naming Rules
- Should start with lowercase.
- CamelCase for multiple words.

```java
public void studentDetails() {}  // Valid
public void StudentDetails() {}  // Valid but discouraged
```

### 6. Identifiers in Java
Identifiers must start with a letter, `_`, or `$` but cannot be keywords.

**Valid Identifiers:** `studentName`, `_value`, `$amount`
**Invalid Identifiers:** `1stValue`, `class`

### 7. White Spaces in Java
Java ignores blank lines and extra spaces for readability.

### 8. Access Modifiers
Java provides access control through modifiers:

| Modifier    | Within Class | Within Package | Subclass (Outside Package) | Outside Package |
|------------|--------------|----------------|-----------------------------|-----------------|
| **private**  | Yes          | No             | No                          | No              |
| **default**  | Yes          | Yes            | No                          | No              |
| **protected**| Yes          | Yes            | Yes                         | No              |
| **public**   | Yes          | Yes            | Yes                         | Yes             |

### 9. Java Keywords
Java has reserved keywords that cannot be used as variable names:

`abstract`, `assert`, `boolean`, `break`, `byte`, `case`, `catch`, `char`, `class`, `continue`, `default`, `do`, `double`, `else`, `enum`, `extends`, `final`, `finally`, `float`, `for`, `goto`, `if`, `implements`, `import`, `instanceof`, `int`, `interface`, `long`, `native`, `new`, `package`, `private`, `protected`, `public`, `return`, `short`, `static`, `strictfp`, `super`, `switch`, `synchronized`, `this`, `throw`, `throws`, `transient`, `try`, `void`, `volatile`, `while`.

---
**Java Programming Guide**

Java is one of the most popular and widely used programming languages and platforms. It is known for being fast, reliable, and secure. Java is utilized in various applications, including web development, desktop applications, mobile applications, gaming consoles, and more. In this article, we will learn how to write and execute a simple Java program.

---

## Steps to Implement a Java Program

The implementation of a Java application involves the following steps:

### 1. Creating the Program
You can create a Java program using a text editor (such as Notepad) or an Integrated Development Environment (IDE) like Eclipse or IntelliJ IDEA.

#### Example Program:
```java
class Demo {
    public static void main(String[] args) {
        System.out.println("My First Java Program.");
    }
}
```
File Save: `D:\Demo.java`

### 2. Compiling the Program
To compile the program, run the Java compiler (`javac`) from the terminal or command prompt:
```
javac Demo.java
```
If the compilation is successful, the Java compiler creates a file called `Demo.class` containing the bytecode of the program.

### 3. Running the Program
To run the compiled Java program, use the following command:
```
java Demo
```
This will output:
```
My First Java Program.
```

---

## Java "Hello, World!" Program
The following is a simple Java program that prints "Hello, World!" to the console.

```java
// This is a simple Java program.
// FileName: "HelloWorld.java"

class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### Output:
```
Hello, World!
```

---

## Explanation of Java Code
### 1. Class Definition
```java
class HelloWorld {
    // Statements
}
```
- Every Java program must have at least one class definition.
- The class name should be capitalized as per naming conventions.

### 2. Main Method
```java
public static void main(String[] args)
```
- **public**: Allows the method to be accessible from anywhere.
- **static**: The method belongs to the class rather than an instance of the class.
- **void**: The method does not return any value.
- **main()**: The standard method name that acts as the entry point for Java programs.
- **String[] args**: Used for command-line arguments.

### 3. Printing to Console
```java
System.out.println("Hello, World!");
```
- `System` is a predefined class that provides system-related operations.
- `out` is an output stream connected to the console.
- `println()` prints the specified string followed by a new line.

---

## Java Syntax Key Elements

### 1. Comments in Java
Comments are used to make code more readable and understandable.

#### Single-line comment:
```java
// This is a single-line comment
```
#### Multi-line comment:
```java
/* This is a
multi-line comment */
```
#### Documentation comment:
```java
/**
 * This is a doc comment
 */
```

### 2. Class Naming Rules
- Class names should start with an uppercase letter.
- Multiple words should follow CamelCase convention.

#### Valid Class Names:
```java
class MyJavaProgram {}  // Valid
class TestProgram {}    // Valid
```
#### Invalid Class Names:
```java
class 1Program {}  // Invalid
```

### 3. Identifiers
Identifiers are names given to variables, methods, classes, etc.
- Must start with a letter, an underscore `_`, or a dollar sign `$`.
- Cannot be a keyword.
- Case-sensitive.

#### Valid Identifiers:
```java
int myVar;
String $name;
boolean is_Valid;
```
#### Invalid Identifiers:
```java
int 2number;  // Invalid (cannot start with a digit)
int class;    // Invalid (reserved keyword)
```

### 4. Access Modifiers
Access modifiers define the visibility and accessibility of classes, methods, and variables.

| Modifier  | Within Class | Within Package | Subclass (Outside Package) | Outside Package |
|-----------|-------------|----------------|----------------------------|-----------------|
| private   | Yes         | No             | No                         | No              |
| default   | Yes         | Yes            | No                         | No              |
| protected | Yes         | Yes            | Yes                        | No              |
| public    | Yes         | Yes            | Yes                        | Yes             |

### 5. Java Keywords
Java has reserved words that cannot be used as identifiers:
```text
abstract, assert, boolean, break, byte, case, catch, char, class, continue, default, do, double, else, enum, extends, final, finally, float, for, goto, if, implements, import, instanceof, int, interface, long, native, new, package, private, protected, public, return, short, static, strictfp, super, switch, synchronized, this, throw, throws, transient, try, void, volatile, while
```

---

## Compiling and Running Java Programs
### Compilation
After setting up the Java environment, open a terminal and navigate to the directory where the file is stored.
To compile a program:
```
javac HelloWorld.java
```
This creates a `HelloWorld.class` file.

### Execution
To run the compiled Java program:
```
java HelloWorld
```
This will print:
```
Hello, World!
```

---

## Conclusion
This guide covers the basics of writing and executing Java programs, including syntax rules, class structure, identifiers, access modifiers, and keywords. Mastering these fundamental concepts is essential for building robust Java applications.

---
---
# Java Identifiers and Reserved Words

## Identifiers in Java
An identifier in Java is the name given to Variables, Classes, Methods, Packages, Interfaces, etc. These are unique names, and every Java variable must be identified with a unique name.

### Example:
```java
public class Test {
    public static void main(String[] args) {
        int a = 20;
    }
}
```
In the above Java code, we have 5 identifiers as follows:

- **Test**: Class Name
- **main**: Method Name
- **String**: Predefined Class Name
- **args**: Variable Name
- **a**: Variable Name

## Rules for Naming Java Identifiers
There are certain rules for defining a valid Java identifier. These rules must be followed, otherwise, a compile-time error occurs. These rules are also valid for other languages like C and C++.

1. The only allowed characters for identifiers are all alphanumeric characters ([A-Z], [a-z], [0-9]), `$` (dollar sign), and `_` (underscore). For example, `geek@` is not a valid Java identifier as it contains a `@`, which is a special character.
2. Identifiers should not start with digits ([0-9]). For example, `123geeks` is not a valid Java identifier.
3. Java identifiers are **case-sensitive**.
4. There is no limit on the length of the identifier, but it is advisable to use an optimum length of 4 – 15 letters.
5. Reserved words cannot be used as identifiers. For example, `int while = 20;` is an invalid statement because `while` is a reserved word. There are 53 reserved words in Java.

### Examples of Valid Identifiers:
```plaintext
MyVariable
MYVARIABLE
myvariable
x
i
x1
i1
_myvariable
$myvariable
sum_of_array
geeks123
```

### Examples of Invalid Identifiers:
```plaintext
My Variable          // contains a space
123geeks            // begins with a digit
a+c                 // plus sign is not an alphanumeric character
variable-2          // hyphen is not an alphanumeric character
sum_&_difference    // ampersand is not an alphanumeric character
```

## Reserved Words in Java
Any programming language reserves some words to represent functionalities defined by that language. These words are called **reserved words**. They can be categorized into two parts:

- **Keywords (50)**: Define functionalities in Java.
- **Literals (3)**: Define constant values.

### Java Keywords:
```plaintext
abstract     continue     for        protected    transient
assert       default      goto       public       try
boolean      do           if         static       throws
break        double       implements strictfp     package
byte         else         import     super        private
case         enum         interface  short        switch
catch        extends      instanceof return       void
char         final        int        synchronized volatile
class        finally      long       throw        date
const        float        native     this         while
```

> **Note:** The keywords `const` and `goto` are reserved, even though they are not currently used. In place of `const`, the `final` keyword is used. Some keywords like `strictfp` were added in later versions of Java.

By following these rules and conventions, you can write clean, readable, and error-free Java code.
---
# Java Keywords

## Introduction
Keywords in Java are reserved words that have predefined meanings and cannot be used as variable names, object names, or identifiers. These keywords play a vital role in defining the syntax and structure of the Java programming language.

## Example: Demonstrating Java Keywords

```java
// Java Program to demonstrate Keywords

class GFG {
    public static void main(String[] args) {
        // Using final and int keyword
        final int x = 10;
        
        // Using if and else keywords
        if (x > 10) {
            System.out.println("Failed");
        } else {
            System.out.println("Successful Demonstration of keywords");
        }
    }
}
```

### Output:
```
Successful Demonstration of keywords
```

## Java Keywords List
Java IDEs and text editors often highlight keywords in different colors to distinguish them from other identifiers. Below is the complete list of Java keywords and their primary usage:

| Keyword    | Usage |
|------------|------------------------------------------------------------------------------------|
| **abstract** | Specifies that a class or method will be implemented later, in a subclass. |
| **assert** | Used for debugging; ensures assumptions in the program are correct. |
| **boolean** | A data type that holds `true` or `false` values. |
| **break** | Exits from a loop or switch statement. |
| **byte** | A data type that holds 8-bit values. |
| **case** | Defines individual conditions in a switch statement. |
| **catch** | Handles exceptions in a try-catch block. |
| **char** | A data type that holds a single 16-bit Unicode character. |
| **class** | Declares a new class. |
| **continue** | Skips the current iteration and moves to the next loop iteration. |
| **default** | Specifies the default case in a switch statement. |
| **do** | Begins a do-while loop. |
| **double** | A data type that holds 64-bit floating-point numbers. |
| **else** | Specifies an alternative block in an `if` statement. |
| **enum** | Declares an enumerated type. |
| **extends** | Indicates that a class inherits from another class. |
| **final** | Declares constants, prevents method overriding, or restricts inheritance. |
| **finally** | Defines a block that executes after a try-catch block. |
| **float** | A data type that holds 32-bit floating-point numbers. |
| **for** | Starts a for loop. |
| **if** | Defines a conditional block. |
| **implements** | Specifies that a class implements an interface. |
| **import** | Imports other Java packages. |
| **instanceof** | Checks whether an object is an instance of a class. |
| **int** | A data type that holds 32-bit integers. |
| **interface** | Declares an interface. |
| **long** | A data type that holds 64-bit integers. |
| **native** | Specifies that a method is implemented using native code. |
| **new** | Creates new objects. |
| **null** | Represents a null reference. |
| **package** | Declares a package. |
| **private** | Defines private access control. |
| **protected** | Defines protected access control. |
| **public** | Defines public access control. |
| **return** | Exits from a method and optionally returns a value. |
| **short** | A data type that holds 16-bit integers. |
| **static** | Declares static methods or variables. |
| **strictfp** | Ensures consistent floating-point calculations across platforms. |
| **super** | Refers to the parent class. |
| **switch** | Implements multi-way branching. |
| **synchronized** | Ensures thread safety by synchronizing methods or blocks. |
| **this** | Refers to the current instance of a class. |
| **throw** | Throws an exception. |
| **throws** | Declares exceptions that a method can throw. |
| **transient** | Specifies that a variable should not be serialized. |
| **try** | Defines a block that can throw exceptions. |
| **void** | Declares a method with no return value. |
| **volatile** | Ensures a variable is read from memory instead of CPU cache. |
| **while** | Begins a while loop. |
| **sealed** | Declares a class with restricted inheritance. |
| **permits** | Specifies allowed subclasses for a sealed class. |

## Example: Using Keywords as Variable Names (Invalid)
Attempting to use a reserved keyword as a variable name will result in an error.

```java
// Java Program to illustrate invalid use of keywords as variable names

class GFG {
    public static void main(String[] args) {
        // "this" is a reserved keyword in Java
        String this = "Hello World!";
        System.out.println(this);
    }
}
```

### Output:
```
Error: not a statement
Error: ';' expected
```

## Important Points:
- `const` and `goto` are reserved keywords but are not used in Java.
- `true`, `false`, and `null` are literals, but they cannot be used as identifiers.

## FAQs – Java Keywords

### What are the keywords in Java?
Keywords are reserved words in Java that have specific meanings and cannot be used as identifiers such as variable names, class names, or object names.

### How many keywords are in Java?
There are **67** keywords in Java, including those introduced in later versions such as `sealed` and `permits`.

### Can we use Java keywords as variable names?
No, Java keywords cannot be used as variable names, method names, or object names.

---
# Java Data Types

## Overview
Java is a **statically typed** and **strongly typed** language, meaning that each type of data (such as integers, characters, and floating-point numbers) is predefined in the programming language. Every variable or constant must be explicitly declared with a specific data type.

Java data types are categorized into two main types:
1. **Primitive Data Types** (e.g., boolean, char, int, short, byte, long, float, double)
2. **Non-Primitive Data Types** (e.g., String, Array, Class, Object, Interface)

## Example of Primitive Data Type:
```java
// Java Program to demonstrate int data-type
class Example {
    public static void main (String[] args) {
        // Declaring two int variables
        int a = 10;
        int b = 20;
        System.out.println(a + b); // Output: 30
    }
}
```

## Primitive Data Types in Java
Primitive data types are the most basic data types in Java, each capable of storing a single value.

| Type    | Description                          | Default  | Size     | Example Literals        | Range |
|---------|--------------------------------------|----------|----------|-------------------------|-------|
| boolean | true or false                       | false    | 1 byte   | true, false             | N/A   |
| byte    | 8-bit signed integer                | 0        | 1 byte   | (none)                   | -128 to 127 |
| char    | 16-bit Unicode character            | '\u0000' | 2 bytes  | 'a', '\u0041', '\n'    | 0 to 65535 |
| short   | 16-bit signed integer               | 0        | 2 bytes  | (none)                   | -32,768 to 32,767 |
| int     | 32-bit signed integer               | 0        | 4 bytes  | -2, -1, 0, 1, 2         | -2,147,483,648 to 2,147,483,647 |
| long    | 64-bit signed integer               | 0L       | 8 bytes  | -2L, -1L, 0L, 1L, 2L    | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 |
| float   | 32-bit IEEE 754 floating-point      | 0.0f     | 4 bytes  | 1.23e10f, -1.23f, 3.14F | Up to 7 decimal digits |
| double  | 64-bit IEEE 754 floating-point      | 0.0d     | 8 bytes  | 1.23456e300d, -1.23d    | Up to 16 decimal digits |

### Example:
```java
// Java Program to Demonstrate Primitive Data Types
class PrimitiveExample {
    public static void main(String[] args) {
        char a = 'G';
        int i = 89;
        byte b = 4;
        short s = 56;
        double d = 4.355453532;
        float f = 4.7333434f;
        long l = 12121;

        System.out.println("char: " + a);
        System.out.println("integer: " + i);
        System.out.println("byte: " + b);
        System.out.println("short: " + s);
        System.out.println("float: " + f);
        System.out.println("double: " + d);
        System.out.println("long: " + l);
    }
}
```
**Output:**
```
char: G
integer: 89
byte: 4
short: 56
float: 4.7333436
double: 4.355453532
long: 12121
```

### Why is the Size of `char` 2 Bytes in Java?
Java uses the **Unicode** character set instead of ASCII, which requires more than 8 bits to represent characters from different languages worldwide. Thus, Java allocates **2 bytes (16 bits)** for `char` to accommodate Unicode characters.

## Non-Primitive (Reference) Data Types
Non-primitive data types hold memory addresses of objects rather than the actual values. These include **String, Class, Object, Interface, and Arrays**.

### 1. **String**
Strings in Java are sequences of characters stored as objects. Unlike C/C++, Java strings are not terminated with a null character (`\0`).

**Syntax:**
```java
String s = "GeeksforGeeks";
String s1 = new String("GeeksforGeeks");
```

### 2. **Class**
A **class** is a blueprint for creating objects, defining properties and methods shared by all instances.

### 3. **Object**
An **object** is an instance of a class, encapsulating state and behavior.

### 4. **Interface**
Interfaces specify a set of methods a class must implement but do not provide implementations themselves.

### 5. **Array**
An **array** is a collection of elements of the same type, indexed for easy access.

**Example:**
```java
int[] arr = {1, 2, 3, 4, 5};
System.out.println(arr[2]); // Output: 3
```

## Key Points to Remember
- **Strong Typing**: Java enforces strict type checking at compile-time, reducing runtime errors.
- **Memory Efficiency**: Choosing the right data type ensures efficient memory usage.
- **Immutability of Strings**: Strings in Java cannot be changed once created, making them thread-safe.
- **Fixed Array Length**: The length of Java arrays is fixed upon declaration and can be accessed using `length`.

## FAQs – Java Data Types

### What are Data Types in Java?
Data types specify the type of data a variable can store, ensuring memory efficiency and type safety.

### What are the 8 Primitive Data Types in Java?
- `boolean`
- `byte`
- `char`
- `short`
- `int`
- `long`
- `float`
- `double`

### Why Does `char` Use 2 Bytes in Java?
Java uses Unicode instead of ASCII, requiring **2 bytes** to store characters from multiple languages.

Understanding Java’s data types is fundamental for efficient programming. Choosing the appropriate type ensures optimal memory usage and program performance while leveraging Java’s strong typing system to catch errors early in development.

---
# Java Variables

## What are Variables in Java?
Variables are containers for storing data values or memory locations for data. Every variable has:

1. **Data Type** – The type of data it holds (e.g., `int`, `String`, `float`, `char`).
2. **Variable Name** – A unique identifier for the variable.
3. **Value** – The data assigned to the variable.

### Example:
```java
int age = 27;       // Integer variable with value 27
String name = "GFG";  // String variable
```

## How to Declare Java Variables?
To declare a variable in Java:
```java
<data_type> <variable_name>;
```
Example:
```java
// Declaring a float variable
float simpleInterest;

// Declaring and initializing integer variable
int time = 10, speed = 20;

// Declaring and initializing character variable
char var = 'h';
```

## Types of Java Variables
Java has three types of variables:
1. **Local Variables**
2. **Instance Variables**
3. **Static Variables**

### 1. Local Variables
- Declared inside a method, constructor, or block.
- Created when the method is called and destroyed after it exits.
- Scope is limited to the block in which it is declared.
- Must be initialized before use.

#### Example:
```java
class GFG {
    public static void main(String[] args) {
        int var = 10; // Local variable
        System.out.println("Local Variable: " + var);
    }
}
```
##### Output:
```
Local Variable: 10
```

---

### 2. Instance Variables
- Declared in a class but outside any method.
- Created when an object is instantiated and destroyed when the object is destroyed.
- Can have access specifiers (default is package-private).
- Initialization is optional (default values depend on data type).

#### Example:
```java
class GFG {
    public String name;
    public int age;

    public GFG() {
        this.name = "Shubham Jain"; // Initializing instance variable
    }

    public static void main(String[] args) {
        GFG obj = new GFG();
        System.out.println("Name: " + obj.name);
        System.out.println("Default value for int: " + obj.age);
    }
}
```
##### Output:
```
Name: Shubham Jain
Default value for int: 0
```

---

### 3. Static Variables
- Declared using the `static` keyword inside a class.
- Belong to the class rather than instances (one copy shared among all objects).
- Created at the start of execution and destroyed when execution ends.
- Can be accessed using the class name.

#### Example:
```java
class GFG {
    static String geek = "Shubham Jain";

    public static void main(String[] args) {
        System.out.println("Geek Name: " + GFG.geek);
    }
}
```
##### Output:
```
Geek Name: Shubham Jain
```

---

## Instance Variables vs Static Variables
| Feature | Instance Variables | Static Variables |
|---------|------------------|----------------|
| Scope | Exists per object | Exists per class |
| Memory | Allocated with object | Allocated once per class |
| Access | Accessed via object | Accessed via class name |
| Lifetime | Created/destroyed with object | Created at start, destroyed at end |

#### Example:
```java
class GFG {
    static int a; // Static variable
    int b;        // Instance variable
}
```

## FAQs – Java Variables

### What are variables in Java?
Variables are memory locations that store data values.

### What are the 3 types of variables in Java?
1. Local Variables
2. Static Variables
3. Instance Variables

### How to declare variables in Java?
Syntax:
```java
<data_type> <variable_name>;
```
Example:
```java
int var1;
---
# Scope of Variables in Java

The **scope of a variable** in Java defines the part of the program where the variable is accessible. Like **C/C++**, Java uses **lexical (or static) scoping**, meaning the scope of a variable is determined at compile time and does not depend on function calls.

## Java Variable Scope Types
The **scope of variables** can be categorized into:

1. **Instance Variables (Class Level Scope)**
2. **Static Variables (Class Level Scope)**
3. **Local Variables (Method Level Scope)**
4. **Parameter Scope**
5. **Block Scope**

---

## 1. Instance Variables – Class Level Scope
- Declared **inside a class but outside any method**.
- Accessible **anywhere within the class**.
- Can have **access modifiers** (public, private, protected, default).
- Can be accessed outside the class if the **access modifier allows it**.

### Example:
```java
public class Test {
    int a; // Instance variable
    private String b; // Private instance variable
    
    void method1() {  }
    int method2() { return a; }
    
    char c;
}
```

### Access Modifiers and Scope
| Modifier  | Package | Subclass | World |
|-----------|---------|----------|--------|
| **public**  | Yes     | Yes      | Yes    |
| **protected** | Yes  | Yes      | No     |
| **default (no modifier)** | Yes | No  | No |
| **private**  | No     | No       | No    |

---

## 2. Static Variables – Class Level Scope
- **Shared across all instances** of a class.
- Declared using the **static** keyword.
- Can be accessed **without creating an instance**.

### Example:
```java
// Using Static Variables
class Test {
    static int var = 10; // Static variable
}

class Geeks {
    public static void main(String[] args) {
        System.out.println("Static Variable: " + Test.var);
    }
}
```
### Output:
```
Static Variable: 10
```

---

## 3. Method Level Scope – Local Variable
- Declared **inside a method**.
- **Not accessible outside the method**.
- **Destroyed** once the method finishes execution.

### Example:
```java
public class Test {
    void method1() {
        int x = 10; // Local variable
        System.out.println(x);
    }
}
```

---

## 4. Parameter Scope – Local Variable
- Variables declared in **method parameters**.
- Exist only during **method execution**.
- Can use **this** keyword to differentiate from instance variables.

### Example:
```java
class Test {
    private int x;
    
    public void setX(int x) {
        this.x = x; // Refers to instance variable
    }
}
```

### Example with Method and Parameter Scope:
```java
public class Geeks {
    static int x = 11; // Class Scope
    private int y = 33; // Instance Variable
    
    public void testFunc(int x) { // Parameter Scope
        Geeks t = new Geeks(); // Method Scope
        this.x = 22;
        y = 44;
        
        System.out.println("Geeks.x: " + Geeks.x);
        System.out.println("t.x: " + t.x);
        System.out.println("t.y: " + t.y);
        System.out.println("y: " + y);
    }
    
    public static void main(String args[]) {
        Geeks t = new Geeks();
        t.testFunc(5);
    }
}
```
### Output:
```
Geeks.x: 22
t.x: 22
t.y: 33
y: 44
```

---

## 5. Block Level Scope
- A variable declared **inside curly braces `{}`** only exists within that block.

### Example:
```java
public class Test {
    public static void main(String args[]) {
        {
            int x = 10;
            System.out.println(x); // Accessible here
        }
        
        // System.out.println(x); // Error: x is out of scope
    }
}
```
### Output:
```
10
```

---

## Incorrect Usage of Local Variables

### 1. Block Level Scope Violation
```java
class Test {
    public static void main(String args[]) {
        int a = 5;
        
        for (int a = 0; a < 5; a++) { // Error: 'a' already defined
            System.out.println(a);
        }
    }
}
```
**Output:**
```
Error: variable 'a' is already defined in method
```

### 2. Accessing Out-of-Scope Variable
```java
class Test {
    public static void main(String args[]) {
        for (int x = 0; x < 4; x++) {
            System.out.println(x);
        }
        
        // System.out.println(x); // Error: x is out of scope
    }
}
```
**Output:**
```
Error: cannot find symbol 'x'
```

---

## Important Points about Variable Scope in Java
✅ **Curly brackets `{}` define the scope**.
✅ A variable can be accessed within the same **or nested brackets** where it was declared.
✅ **Class variables** (outside methods) can be used in all member methods.
✅ Use **this** keyword to refer to instance variables when a method parameter has the same name.
✅ To access a variable **after a loop**, declare it **before the loop**.

---

## FAQs – Java Variable Scope
### 1. What is the Scope of Variables in Java?
The **scope of a variable** defines the region of the program where it can be accessed.

### 2. How many types of Scope exist in Java?
There are **five** types:
- **Local Scope**
- **Instance Scope**
- **Class Scope (Static Scope)**
- **Parameter Scope**
- **Block Scope**

### 3. Will this program run successfully?
```java
class Test {
    public static void main(String args[]) {
        for (int i = 1; i <= 10; i++) {
            System.out.print(i + " ");
        }
        
        int i = 20; // New variable after loop
        System.out.print(i + " ");
    }
}
```
✅ **Yes, it will run** because the loop variable `i` is destroyed before declaring a new `i`.

### Output:
```
1 2 3 4 5 6 7 8 9 10 20
```

---
### 🎯 **Summary**
Understanding **variable scope** is crucial for writing efficient and bug-free Java code. Using correct **local, instance, static, and block scopes** helps in avoiding **naming conflicts** and **reducing memory usage**.

Happy Coding! 🚀

---
# Java Operators

Java operators are special symbols that perform operations on variables or values. They can be classified into several categories based on their functionality. These operators play a crucial role in performing arithmetic, logical, relational, and bitwise operations, etc.

## Example: Using `+` and `-` operators

```java
public class Geeks
{  
    public static void main(String[] args)
    {
        // Declare and initialize variables
        int num1 = 500;
        int num2 = 100;
        
        // Using the + (addition) operator
        int sum = num1 + num2;
        System.out.println("The Sum is: "+sum);
        
        // Using the - (subtraction) operator
        int diff = num1 - num2;
        System.out.println("The Difference is: "+diff);
    }
}
```
### Output:
```
The Sum is: 600
The Difference is: 400
```

---

## Types of Operators in Java
1. **Arithmetic Operators**
2. **Unary Operators**
3. **Assignment Operators**
4. **Relational Operators**
5. **Logical Operators**
6. **Ternary Operator**
7. **Bitwise Operators**
8. **Shift Operators**
9. **`instanceof` Operator**

---

## 1. Arithmetic Operators
Arithmetic Operators are used to perform simple arithmetic operations on primitive and non-primitive data types.

| Operator | Description       |
|----------|------------------|
| `*`      | Multiplication   |
| `/`      | Division         |
| `%`      | Modulo           |
| `+`      | Addition         |
| `-`      | Subtraction      |

### Example:
```java
class Geeks
{
    public static void main (String[] args)
    {
        int a = 10;
        int b = 3;
        System.out.println("a + b = " + (a + b));
        System.out.println("a - b = " + (a - b));
        System.out.println("a * b = " + (a * b));
        System.out.println("a / b = " + (a / b));
        System.out.println("a % b = " + (a % b));
    }
}
```

### Output:
```
a + b = 13
a - b = 7
a * b = 30
a / b = 3
a % b = 1
```

---

## 2. Unary Operators
Unary Operators operate on a single operand. They include:

| Operator | Description |
|----------|------------|
| `-`      | Negation   |
| `+`      | Positive indication |
| `++`     | Increment (pre/post) |
| `--`     | Decrement (pre/post) |
| `!`      | Logical NOT |

### Example:
```java
class Geeks {
    public static void main(String[] args)
    {
        int a = 10;
        System.out.println("Postincrement : " + (a++));
        System.out.println("Preincrement : " + (++a));
        System.out.println("Postdecrement : " + (a--));
        System.out.println("Predecrement : " + (--a));
    }
}
```

### Output:
```
Postincrement : 10
Preincrement : 12
Postdecrement : 12
Predecrement : 10
```

---

## 3. Assignment Operators
Assignment operators assign values to variables.

| Operator | Example | Equivalent To |
|----------|---------|--------------|
| `=`      | a = b  | Assign b to a |
| `+=`     | a += b | a = a + b |
| `-=`     | a -= b | a = a - b |
| `*=`     | a *= b | a = a * b |
| `/=`     | a /= b | a = a / b |
| `%=`     | a %= b | a = a % b |

### Example:
```java
class Geeks {
    public static void main(String[] args) {
        int f = 7;
        System.out.println("f += 3: " + (f += 3));
        System.out.println("f -= 2: " + (f -= 2));
        System.out.println("f *= 4: " + (f *= 4));
        System.out.println("f /= 3: " + (f /= 3));
    }
}
```

---

## 4. Relational Operators
Used to compare values and return boolean results.

| Operator | Description |
|----------|------------|
| `==`     | Equal to |
| `!=`     | Not equal to |
| `<`      | Less than |
| `<=`     | Less than or equal to |
| `>`      | Greater than |
| `>=`     | Greater than or equal to |

---

## 5. Logical Operators
Used in boolean logic.

| Operator | Description |
|----------|------------|
| `&&`     | Logical AND |
| `||`     | Logical OR |
| `!`      | Logical NOT |

### Example:
```java
class Geeks {
    public static void main (String[] args) {
        boolean x = true;
        boolean y = false;
        System.out.println("x && y: " + (x && y));
        System.out.println("x || y: " + (x || y));
        System.out.println("!x: " + (!x));
    }
}
```

---

## 6. Ternary Operator
Shorthand for `if-else`.

```java
result = (condition) ? if_true : if_false;
```

### Example:
```java
public class Geeks {
    public static void main(String[] args)
    {
        int a = 20, b = 10, c = 30;
        int result = ((a > b) ? (a > c ? a : c) : (b > c ? b : c));
        System.out.println("Max of three numbers = " + result);
    }
}
```

---

## 7. Bitwise Operators
Used for bitwise operations.

| Operator | Description |
|----------|------------|
| `&`      | Bitwise AND |
| `|`      | Bitwise OR |
| `^`      | Bitwise XOR |
| `~`      | Bitwise Complement |

---

## 8. Shift Operators

| Operator | Description |
|----------|------------|
| `<<`     | Left shift |
| `>>`     | Right shift |
| `>>>`    | Unsigned right shift |

---

## 9. `instanceof` Operator
Used for type checking.

```java
object instanceof class/subclass/interface
```

# Java User Input

The most common way to take user input in Java is by using the **Scanner** class, which is part of the `java.util` package. The Scanner class can read input from various sources like **console, files, or streams**. It was introduced in **Java 5**. Before that, the **BufferedReader** class (introduced in Java 1.1) was used.

As a beginner, we recommend using the **Scanner** class for its simplicity.

---
## Using Scanner Class

### Steps to Take User Input
1. **Import the Scanner class** using `import java.util.Scanner;`
2. **Create a Scanner object** and connect it to `System.in`:
   ```java
   Scanner scn = new Scanner(System.in);
   ```
3. **Use methods of the Scanner class** (e.g., `nextInt()`, `nextLine()`, `next()`, `nextDouble()`, etc.) to read user input.

### Example 1: Taking Integer Input
```java
import java.util.Scanner;

class Geeks {
    public static void main(String[] args) {
        // Creating Scanner object
        Scanner scn = new Scanner(System.in);
        
        // Enter first input
        System.out.print("Enter First Number: ");
        int a = scn.nextInt();
        
        System.out.print("Enter Second Number: ");
        int b = scn.nextInt();
        
        System.out.println("Sum: " + (a + b));
        
        // Closing the scanner to release resources
        scn.close();
    }
}
```
#### **Output:**
```
Enter First Number: 2
Enter Second Number: 3
Sum: 5
```

---
## Scanner Class Methods

| Method         | Description                              |
|---------------|-----------------------------------------|
| `nextBoolean()` | Reads a Boolean value (`true` or `false`). |
| `nextByte()`    | Reads a Byte value.                     |
| `nextDouble()`  | Reads a Double value.                   |
| `nextFloat()`   | Reads a Float value.                    |
| `nextInt()`     | Reads an Integer value.                 |
| `nextLine()`    | Reads an entire line.                   |
| `nextLong()`    | Reads a Long value.                     |
| `nextShort()`   | Reads a Short value.                    |

---
## Example 2: Taking Multiple Inputs
```java
import java.util.Scanner;

class Geeks {
    public static void main(String[] args) {
        // Scanner object
        Scanner scn = new Scanner(System.in);

        // Read a single word
        System.out.print("Enter a word: ");
        String str1 = scn.next();
        System.out.println("Entered String: " + str1);

        scn.nextLine(); // Consume the newline left by next()
        
        // Read a full sentence
        System.out.print("Enter a sentence: ");
        String str2 = scn.nextLine();
        System.out.println("Entered Sentence: " + str2);

        // Read an integer
        System.out.print("Enter an Integer: ");
        int x = scn.nextInt();
        System.out.println("Entered Integer: " + x);

        // Read a float
        System.out.print("Enter a Float value: ");
        float f = scn.nextFloat();
        System.out.println("Entered Float Value: " + f);
    }
}
```
#### **Output:**
```
Enter a word: Geeks
Entered String: Geeks
Enter a sentence: Geeks For Geeks
Entered Sentence: Geeks For Geeks
Enter an Integer: 123
Entered Integer: 123
Enter a Float value: 123.090
Entered Float Value: 123.09
```

---
## Using BufferedReader Class
Another way to take user input is by using **BufferedReader**. It is useful for reading a sequence of characters efficiently. 

### BufferedReader Methods
| Method                 | Description                                  |
|------------------------|----------------------------------------------|
| `read()`              | Reads a single character.                    |
| `read(char[] cbuf)`   | Reads an array of characters.                |
| `readLine()`          | Reads an entire line of text.                |

### Example:
```java
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;

class BufferedReaderExample {
    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        
        System.out.print("Enter your name: ");
        String name = br.readLine();
        
        System.out.println("Hello, " + name + "!");
    }
}
```
#### **Output:**
```
Enter your name: Raj
Hello, Raj!
```

---
## BufferedReader vs Scanner Class

| Aspects            | BufferedReader                          | Scanner                           |
|--------------------|--------------------------------------|----------------------------------|
| **Primary Use**    | Efficient reading of character streams. | Reading formatted input (integers, strings). |
| **Speed**         | Faster for large input (less parsing). | Slower due to parsing overhead. |
| **Exception Handling** | Throws checked exceptions (IOException). | No checked exceptions, easier to use. |
| **Flexibility**    | Better for larger input files.         | Best for simple data types. |
| **Thread Safety**  | Synchronized, thread-safe.             | Not thread-safe. |

---
## Common Scanner Issues
### **Problem: `nextLine()` After `nextInt()` or `nextFloat()`**
When you use `nextInt()` or `nextFloat()`, it reads the number but leaves a **newline character** (`\n`) in the input buffer. If you call `nextLine()` immediately after, it reads this leftover newline instead of waiting for new input.

### **Solution:**
```java
Scanner sc = new Scanner(System.in);

// Read integer
System.out.print("Enter an integer: ");
int num = sc.nextInt();

// Consume newline character
sc.nextLine();  

// Read string input
System.out.print("Enter your name: ");
String name = sc.nextLine();

System.out.println("Number: " + num);
System.out.println("Name: " + name);
```

---
## **FAQs – Java User Input**

### **What are the different ways to take input in Java?**
1. **BufferedReader** – Efficient for large input.
2. **Scanner** – Simple and commonly used.
3. **Console** – Used for password inputs (does not work in IDEs like Eclipse).

### **Is Scanner thread-safe?**
No, **Scanner is not thread-safe**. If used in a multi-threaded environment, synchronization is required, or `BufferedReader` should be used.

### **When should I use BufferedReader instead of Scanner?**
Use **BufferedReader** when:
- Handling large input.
- Avoiding parsing overhead.
- Needing **thread safety**.

Use **Scanner** when:
- Reading simple data types.
- No need for multi-threading.

---
That’s all about **Java User Input**! 🎯 Happy Coding! 🚀
---
# Java Flow Control

## If Statement in Java
The `if` statement is the simplest decision-making statement in Java. It is used to decide whether a block of statements should be executed or not based on a condition.

### Example:
```java
// Java program to illustrate If statement
class GfG {
    public static void main(String args[]) {
        int i = 10;

        // using if statement
        if (i < 15)
            System.out.println("10 is less than 15");

        System.out.println("Outside if-block");
    }
}
```

### Output:
```
10 is less than 15
Outside if-block
```

### Dry-Running the Example:
1. Program starts.
2. `i` is initialized to `10`.
3. The if-condition `10 < 15` is checked, which is `true`.
   - "10 is less than 15" is printed.
4. "Outside if-block" is printed.

### Syntax:
```java
if (condition) {
   // Statements to execute if condition is true
}
```

### Working of `if` Statement:
1. Control falls into the `if` block.
2. The condition is tested.
3. If the condition evaluates to `true`, the body inside the `if` is executed.
4. If the condition evaluates to `false`, the `if` block is skipped.
5. The flow then moves to the next statement outside the `if` block.

### Important Note:
If curly braces `{}` are omitted, the `if` statement considers only the immediate next statement as its body.

#### Example:
```java
if(condition)
   statement1;
   statement2;
```
- Here, if the condition is `true`, only `statement1` is executed under `if`.
- `statement2` is always executed, regardless of the condition.

## Example 1: Using `if` Statement
```java
// Java program to illustrate If statement
class GFG {
    public static void main(String args[]) {
        String str = "GeeksforGeeks";
        int i = 4;

        // if block
        if (i == 4) {
            i++;
            System.out.println(str);
        }

        // Executed by default
        System.out.println("i = " + i);
    }
}
```

### Output:
```
GeeksforGeeks
i = 5
```

## Example 2: Implementing `if-else` for Boolean Values

### Input:
```java
boolean a = true;
boolean b = false;
```

### Example Code:
```java
// Java program to illustrate the if-else statement
public class IfElseExample {
    public static void main(String[] args) {
        boolean a = true;
        boolean b = false;
        
        if (a) {
            System.out.println("a is true");
        } else {
            System.out.println("a is false");
        }
        
        if (b) {
            System.out.println("b is true");
        } else {
            System.out.println("b is false");
        }
    }
}
```

### Output:
```
a is true
b is false
```

### Explanation:
1. `boolean a = true;` and `boolean b = false;` are initialized.
2. The first `if-else` checks `a`:
   - Since `a` is `true`, it prints `"a is true"`.
3. The second `if-else` checks `b`:
   - Since `b` is `false`, it prints `"b is false"`.

This demonstrates how to use `if-else` statements for making decisions based on Boolean values.

## Advantages of `if-else` Statement:
1. **Conditional Execution**: Executes a block of code based on a Boolean condition.
2. **Readability**: Improves code readability by clearly showing when a block should execute.
3. **Reusability**: Can be used multiple times across different parts of a program.
4. **Debugging**: Helps trace logic errors by clearly defining conditions.
5. **Flexibility**: Allows handling of different scenarios dynamically.

The `if-else` statement is a fundamental concept in Java programming that helps control the flow of execution efficiently.
---
# Java if-else Statement

The **if-else** statement in Java is a powerful decision-making tool used to control the program’s flow based on conditions. It executes one block of code if a condition is **true** and another block if the condition is **false**. In this article, we will learn about Java if-else statements with examples.

## Example of if-else Statement

```java
// Java Program to demonstrate if-else statement
public class IfElse {
    public static void main(String[] args) {
        int n = 10;

        if (n > 5) {
            System.out.println("The number is greater than 5.");
        } else {
            System.out.println("The number is 5 or less.");
        }
    }
}
```

### Output
```
The number is greater than 5.
```

### Dry-Running the Example
1. The program starts.
2. `n` is initialized to **10**.
3. The **if** condition is checked: `10 > 5`, which is **true**.
4. The block inside the **if** statement executes: `"The number is greater than 5."` is printed.
5. The **else** block is skipped since the condition is true.

## Syntax of if-else Statement

```java
if (condition) {
    // Executes this block if condition is true
} else {
    // Executes this block if condition is false
}
```

### Working of if-else Statement
1. Control falls into the **if** block.
2. The flow jumps to the **condition**.
3. The condition is tested:
   - If **true**, the **if** block executes.
   - If **false**, the **else** block executes.
4. Control exits the **if-else** block and continues the program.

## Nested if Statement in Java
In Java, we can use **nested if statements** to create more complex conditional logic. A nested if statement is an **if statement inside another if statement**.

### Syntax of Nested if
```java
if (condition1) {
    // Code block 1
    if (condition2) {
        // Code block 2
    }
}
```

### Example of Nested if Statement

```java
// Java Program to implement Nested if statement
public class NestedIf {
    public static void main(String[] args) {
        int age = 25;
        double weight = 65.5;

        if (age >= 18) {
            if (weight >= 50.0) {
                System.out.println("You are eligible to donate blood.");
            } else {
                System.out.println("You must weigh at least 50 kilograms to donate blood.");
            }
        } else {
            System.out.println("You must be at least 18 years old to donate blood.");
        }
    }
}
```

### Output
```
You are eligible to donate blood.
```

### Important Notes
- The **else** statement cannot exist without an **if** statement.
- If there is no **else** block, the program simply skips the **if** block if the condition is false.
- Multiple **if-else** statements can be used in a program.
- **Nested if statements** allow handling more complex conditions.

## Java if-else Statement – FAQs

### What is the if-else Statement in Java?
The **if-else** statement in Java allows executing one block of code when a condition is **true** and another block when the condition is **false**.

### What is the Syntax for if-else Statement?
```java
if (condition) {
    // Executes this block if condition is true
} else {
    // Executes this block if condition is false
}
```

### Can an else Block Exist Without an if Statement?
No, an **else** block must always be associated with an **if** statement. It cannot exist independently.

### What Happens if the if Condition is False and There is No else Block?
If the **if** condition evaluates to **false** and there is no **else** block, the program simply skips the **if** block and continues execution with the next statement.

### Can We Use Multiple if-else Statements in a Program?
Yes, multiple **if-else** statements can be used, and they can also be **nested** to handle complex decision-making.

---
# Java if-else-if Ladder with Examples

## Overview
The Java **if-else-if ladder** is used to evaluate multiple conditions sequentially. It allows a program to check several conditions and execute the block of code associated with the first true condition. If none of the conditions are true, an optional `else` block can execute as a fallback.

## Example
The below example demonstrates a straightforward if-else-if ladder structure. It evaluates a number and prints the corresponding message based on the condition.

```java
// Java program to demonstrate a simple if-else-if ladder
class GFG {
    public static void main(String[] args) {
        int i = 20;

        // if-else-if ladder to check the value of i
        if (i == 10)
            System.out.println("i is 10");
        else if (i == 20)
            System.out.println("i is 20");
        else
            System.out.println("i is neither 10 nor 20");
    }
}
```

### Output
```
i is 20
```

### Dry-Running the Above Example
1. The program starts.
2. `i` is initialized to `20`.
3. The first `if` condition `i == 10` is checked:
   - It evaluates to `false` because `i` is `20`.
4. The second `else if` condition `i == 20` is checked:
   - It evaluates to `true` because `i` is `20`.
   - `"i is 20"` is printed.
5. The `else` block is skipped since a condition was satisfied.
6. The program ends.

---

## Syntax of if-else-if Ladder
```java
if (condition)
    statement1;
else if (condition)
    statement2;
...
else
    statement;
```

## Working of the if-else-if Ladder
1. Control falls into the `if` block.
2. The first condition is tested.
   - If `true`, execute the associated block and exit the ladder.
   - If `false`, move to the next `else if` condition.
3. Repeat step 2 until a `true` condition is found.
4. If none of the conditions are `true`, execute the `else` block.
5. Exit the if-else-if ladder.

## Example 1: Using the if-else-if Ladder

```java
// Java program to illustrate if-else-if ladder
class GFG {
    public static void main(String[] args) {
        int i = 20;

        // condition 1
        if (i == 10)
            System.out.println("i is 10");

        // condition 2
        else if (i == 15)
            System.out.println("i is 15");

        // condition 3
        else if (i == 20)
            System.out.println("i is 20");

        else
            System.out.println("i is not present");

        System.out.println("Outside if-else-if");
    }
}
```

### Output
```
i is 20
Outside if-else-if
```

### Explanation
- The if-else-if ladder checks multiple conditions sequentially.
- Since `i == 20`, the corresponding statement is printed.
- The `else` block is skipped as a condition was satisfied.

---

## Advantages of Java if-else-if Ladder

1. **Sequential Condition Checking**: Evaluates multiple conditions in order, making it useful for handling a range of scenarios.
2. **Readability**: Easy to read and understand for simple decision-making logic.
3. **Fallback Mechanism**: Provides an optional `else` block to handle cases where none of the conditions are met.
4. **Versatile**: Can be used for both numerical and logical comparisons.
5. **Simpler Alternative**: Suitable for situations where using `switch` is not feasible, such as complex conditions.

---

The **if-else-if ladder** is a fundamental control structure in Java, helping developers handle multiple conditions efficiently.
---
# Java for Loop with Examples

## Introduction
The **for loop** in Java is a control flow statement that allows code to be executed repeatedly based on a given condition. It provides an efficient way to iterate over a range of values, execute code multiple times, or traverse arrays and collections.

---

## Syntax of for Loop
```java
for (initialization; condition; update) {
    // Loop body
    // Statements to execute
}
```

### Explanation:
1. **Initialization:** The loop variable is initialized once before the loop starts.
2. **Condition:** The loop runs as long as this condition is `true`.
3. **Update:** After each iteration, the loop variable is updated (incremented/decremented).

---

## Example 1: Printing Numbers from 1 to 5
```java
class Geeks {
    public static void main(String args[]) {
        for (int i = 1; i <= 5; i++) {
            System.out.println(i);
        }
        System.out.println("Loop has ended.");
    }
}
```
### Output:
```
1
2
3
4
5
Loop has ended.
```

### Dry Run:
1. **i = 1** → Condition `i <= 5` is `true`, prints `1`, `i++`.
2. **i = 2** → Condition `true`, prints `2`, `i++`.
3. **i = 3** → Condition `true`, prints `3`, `i++`.
4. **i = 4** → Condition `true`, prints `4`, `i++`.
5. **i = 5** → Condition `true`, prints `5`, `i++`.
6. **i = 6** → Condition `false`, exits loop, prints "Loop has ended."

---

## Example 2: Printing "Hello World" 5 Times
```java
class GFG {
    public static void main(String args[]) {
        for (int i = 1; i <= 5; i++) {
            System.out.println("Hello World");
        }
    }
}
```
### Output:
```
Hello World
Hello World
Hello World
Hello World
Hello World
```

---

## Example 3: Calculating Sum from 1 to 20
```java
class GFG {
    public static void main(String args[]) {
        int sum = 0;
        for (int x = 1; x <= 20; x++) {
            sum = sum + x;
        }
        System.out.println("Sum: " + sum);
    }
}
```
### Output:
```
Sum: 210
```

---

## Nested for Loop
A **nested for loop** is a for loop inside another for loop. It is commonly used for multidimensional problems.

### Example: Printing a Matrix-like Pattern
```java
class GFG {
    public static void main(String[] args) {
        for (int i = 1; i <= 3; i++) {
            for (int j = 1; j <= 3; j++) {
                System.out.print("(" + i + "," + j + ") ");
            }
            System.out.println();
        }
    }
}
```
### Output:
```
(1,1) (1,2) (1,3)
(2,1) (2,2) (2,3)
(3,1) (3,2) (3,3)
```

---

## Java Infinite for Loop
An **infinite loop** occurs when the loop's condition never becomes false.

### Example 1:
```java
class GFG {
    public static void main(String args[]) {
        for (int i = 1; i >= 1; i++) {
            System.out.println("Infinite Loop " + i);
        }
    }
}
```
### Output:
```
Infinite Loop 1
Infinite Loop 2
...
```

### Example 2: Using Empty Condition
```java
class GFG {
    public static void main(String[] args) {
        for (;;) {
            System.out.println("Infinite Loop");
        }
    }
}
```
### Output:
```
Infinite Loop
Infinite Loop
...
```
**Note:** This will cause a "Time Limit Exceeded" error if not stopped manually.

---

## Advantages of for Loop
1. **Efficient Iteration:** Ideal for looping through a known range.
2. **Compact Syntax:** Initialization, condition, and update in one line.
3. **Easy to Control:** Allows easy increment/decrement.
4. **Useful for Collections:** Works well for arrays and lists.

---

## Conclusion
The `for` loop is a powerful iteration statement in Java. It provides a concise way to loop through a sequence, making it essential for programming logic, numerical computations, and collection traversal.

---

Happy Coding! 🚀

---
# Java For-Each Loop (Enhanced For Loop)

The **for-each loop** in Java (also called the **enhanced for loop**) was introduced in **Java 5** to simplify iteration over arrays and collections. It is more **concise, readable, and avoids common indexing errors** that occur in traditional loops.

## Advantages of For-Each Loop
- **Simpler syntax** compared to traditional for-loops.
- **Avoids index management** since it directly accesses elements.
- **Prevents out-of-bounds errors** as it only iterates within the valid range.
- **More readable** and clean.

## Syntax
```java
for (dataType variable : collection) {
    // Statements using variable
}
```

## Example 1: Iterating Over an Array
```java
// Java Program to Iterate through an array using for-each loop
class ForEachExample {
    public static void main(String[] args) {
        int[] arr = {1, 2, 3, 4, 5};
        
        // Using for-each loop to print each element
        for (int num : arr) {
            System.out.print(num + " ");
        }
    }
}
```
### **Output**
```
1 2 3 4 5
```

## Example 2: Finding Maximum in an Array
```java
// Java Program to find maximum in an array using for-each loop
public class MaximumFinder {
    public static void main(String[] args) {
        int[] marks = {125, 132, 95, 116, 110};
        int max = findMax(marks);
        System.out.println("Maximum: " + max);
    }

    public static int findMax(int[] numbers) {
        int maximum = numbers[0];
        for (int num : numbers) {
            if (num > maximum) {
                maximum = num;
            }
        }
        return maximum;
    }
}
```
### **Output**
```
Maximum: 132
```

## Limitations of For-Each Loop
While the for-each loop is convenient, there are some important **limitations** to consider:

### 1. **Cannot Modify Array Elements Directly**
```java
int[] marks = {10, 20, 30};
for (int num : marks) {
    num = num * 2; // Modifies only 'num', not actual array elements
}
```
**Explanation**: The for-each loop provides a **copy** of each element, so changes do not affect the original array.

### 2. **No Access to Index**
```java
for (int num : numbers) {
    if (num == target) {
        // Cannot get the index of 'num'
        return ???; 
    }
}
```
**Explanation**: The for-each loop **does not provide an index**, making it difficult to find an element’s position.

### 3. **Single-Direction Iteration Only**
```java
for (int i = numbers.length - 1; i >= 0; i--) {
    System.out.println(numbers[i]);
}
```
**Explanation**: The for-each loop **only iterates forward**, so for **reverse iteration**, a traditional loop is needed.

### 4. **Complex Conditions Are Difficult to Implement**
```java
for (int i = 0; i < numbers.length; i++) {
    if (numbers[i] == arr[i]) {
        // Complex checks easier in a traditional for loop
    }
}
```
**Explanation**: If our logic requires checking multiple conditions or using indices, a traditional for-loop offers more flexibility.

### 5. **Performance Overhead**
For-each loops may have **slight performance drawbacks** when working with large collections due to **hidden iterator overhead**.

```java
import java.util.*;

class LoopPerformanceComparison {
    public static void main(String[] args) {
        List<Integer> list = new ArrayList<>();
        for (int i = 0; i < 1000000; i++) list.add(i);
        
        long startTime, endTime;

        // Type 1: Using a for-each loop
        startTime = System.currentTimeMillis();
        for (int num : list) { int a = num; }
        endTime = System.currentTimeMillis();
        System.out.println("For-each loop: " + (endTime - startTime) + " ms");

        // Type 2: Using list.size() in the loop condition
        startTime = System.currentTimeMillis();
        for (int j = 0; j < list.size(); j++) { int a = list.get(j); }
        endTime = System.currentTimeMillis();
        System.out.println("Using list.size(): " + (endTime - startTime) + " ms");

        // Type 3: Calculating list size before the loop
        startTime = System.currentTimeMillis();
        int size = list.size();
        for (int j = 0; j < size; j++) { int a = list.get(j); }
        endTime = System.currentTimeMillis();
        System.out.println("Precomputed list.size(): " + (endTime - startTime) + " ms");

        // Type 4: Iterating in reverse order
        startTime = System.currentTimeMillis();
        for (int j = list.size() - 1; j >= 0; j--) { int a = list.get(j); }
        endTime = System.currentTimeMillis();
        System.out.println("Reverse iteration: " + (endTime - startTime) + " ms");
    }
}
```
### **Output (Example Execution)**
```
For-each loop: 85 ms
Using list.size(): 11 ms
Precomputed list.size(): 33 ms
Reverse iteration: 19 ms
```

## Key Points to Remember
- **Simplifies iteration** over arrays and collections.
- **No index access**, making it less useful when modifying elements.
- **Cannot iterate in reverse order**.
- **Might have slight performance overhead** due to iterators.
- **Recommended for cases where element access is required without index tracking.**

---
That’s everything about the **for-each loop** in Java! 🚀
---
# Java do-while Loop

The **Java do-while loop** is an exit-controlled loop that ensures the execution of the loop body at least once before checking the condition. Unlike `for` or `while` loops, which test the condition before executing the loop body, `do-while` checks the condition after executing the statements inside the loop body.

---

## Syntax of do-while Loop

```java
do {
    // Loop Body
    Update_expression;
} while (test_expression);
```

**Note:** The `test_expression` in the `do-while` loop must return a boolean value; otherwise, a compile-time error will occur.

---

## Execution Flow of do-while Loop

1. Control enters the `do-while` loop.
2. The statements inside the body of the loop execute.
3. The **update expression** modifies the loop variable.
4. The **condition** is tested.
   - If **true**, the loop body executes again.
   - If **false**, the loop terminates, and execution continues with the next statement after the loop.

---

## Example: Basic do-while Loop

```java
// Java program demonstrating do-while loop
public class DoWhileExample {
    public static void main(String[] args) {
        int c = 1;

        do {
            System.out.println("Java do-while Loop: " + c);
            c++;
        } while (c <= 5);
    }
}
```

### Output:
```
Java do-while Loop: 1
Java do-while Loop: 2
Java do-while Loop: 3
Java do-while Loop: 4
Java do-while Loop: 5
```

---

## Practical Application of do-while Loop

A `do-while` loop is useful when we want to execute a set of statements **at least once**, regardless of the condition. A common example is displaying a menu in a game or an application where options must be shown at least once before accepting user input.

---

## Example: do-while Ensuring One-Time Execution

```java
// Java Program to Illustrate One-Time Execution in do-while
public class OneTimeExecution {
    public static void main(String[] args) {
        int c = 0;

        do {
            System.out.println("Print Statement");
            c++;
        } while (c < 0);
    }
}
```

### Output:
```
Print Statement
```

### Explanation:
Since the condition `(c < 0)` is **false**, the loop body still executes **once** before terminating.

---

## Components of do-while Loop

1. **Test Expression:** This is the condition that controls the loop execution.
   - Example: `i <= 10`
2. **Update Expression:** This updates the loop variable to avoid infinite loops.
   - Example: `i++`

---

## Example 1: Printing a Message Multiple Times

```java
// Java Program to Print "Hello World" 5 times using do-while loop
public class HelloWorldExample {
    public static void main(String[] args) {
        int c = 1;
        
        do {
            System.out.println("Hello World");
            c++;
        } while (c < 6);
    }
}
```

### Output:
```
Hello World
Hello World
Hello World
Hello World
Hello World
```

### Execution Steps:
1. `c` is initialized with `1`.
2. "Hello World" gets printed.
3. `c` is incremented.
4. The condition `c < 6` is checked.
5. If true, the loop continues; if false, it terminates.

---

## Example 2: do-while Loop Without Curly Braces `{}`

```java
// Java program demonstrating do-while loop without curly braces
public class WithoutBraces {
    public static void main(String[] args) {
        int c = 1;
        
        do
            System.out.println("Hello Java!");
        while (c >= 3); // Condition is false, but the loop runs once
    }
}
```

### Output:
```
Hello Java!
```

### Explanation:
Since there is **only one statement** inside the `do` block, curly braces `{}` are optional. The loop executes **once** before checking the condition `(c >= 3)`, which is false.

---

## When to Use do-while Loop?

- When **at least one execution** is required before checking the condition.
- When displaying a **menu-driven system**.
- When handling **user input loops** that must execute at least once.

---

## Summary

| Feature             | while Loop | do-while Loop |
|---------------------|------------|--------------|
| Condition Check     | Before execution | After execution |
| Minimum Executions | **0** (if false initially) | **At least 1** |
| Use Case | When execution depends on a condition | When execution must happen at least once |

The `do-while` loop is a useful construct in Java that ensures at least one execution of the loop body before checking the condition. This is especially beneficial for interactive programs like games, menus, or situations where input validation is required.

---

# Java do-while Loop

The **Java do-while loop** is an exit-controlled loop that ensures the execution of the loop body at least once before checking the condition. Unlike `for` or `while` loops, which test the condition before executing the loop body, `do-while` checks the condition after executing the statements inside the loop body.

---

## Syntax of do-while Loop

```java
do {
    // Loop Body
    Update_expression;
} while (test_expression);
```

**Note:** The `test_expression` in the `do-while` loop must return a boolean value; otherwise, a compile-time error will occur.

---

## Execution Flow of do-while Loop

1. Control enters the `do-while` loop.
2. The statements inside the body of the loop execute.
3. The **update expression** modifies the loop variable.
4. The **condition** is tested.
   - If **true**, the loop body executes again.
   - If **false**, the loop terminates, and execution continues with the next statement after the loop.

---

## Example: Basic do-while Loop

```java
// Java program demonstrating do-while loop
public class DoWhileExample {
    public static void main(String[] args) {
        int c = 1;

        do {
            System.out.println("Java do-while Loop: " + c);
            c++;
        } while (c <= 5);
    }
}
```

### Output:
```
Java do-while Loop: 1
Java do-while Loop: 2
Java do-while Loop: 3
Java do-while Loop: 4
Java do-while Loop: 5
```

---

## Practical Application of do-while Loop

A `do-while` loop is useful when we want to execute a set of statements **at least once**, regardless of the condition. A common example is displaying a menu in a game or an application where options must be shown at least once before accepting user input.

---

## Example: do-while Ensuring One-Time Execution

```java
// Java Program to Illustrate One-Time Execution in do-while
public class OneTimeExecution {
    public static void main(String[] args) {
        int c = 0;

        do {
            System.out.println("Print Statement");
            c++;
        } while (c < 0);
    }
}
```

### Output:
```
Print Statement
```

### Explanation:
Since the condition `(c < 0)` is **false**, the loop body still executes **once** before terminating.

---

## Components of do-while Loop

1. **Test Expression:** This is the condition that controls the loop execution.
   - Example: `i <= 10`
2. **Update Expression:** This updates the loop variable to avoid infinite loops.
   - Example: `i++`

---

## Example 1: Printing a Message Multiple Times

```java
// Java Program to Print "Hello World" 5 times using do-while loop
public class HelloWorldExample {
    public static void main(String[] args) {
        int c = 1;
        
        do {
            System.out.println("Hello World");
            c++;
        } while (c < 6);
    }
}
```

### Output:
```
Hello World
Hello World
Hello World
Hello World
Hello World
```

### Execution Steps:
1. `c` is initialized with `1`.
2. "Hello World" gets printed.
3. `c` is incremented.
4. The condition `c < 6` is checked.
5. If true, the loop continues; if false, it terminates.

---

## Example 2: do-while Loop Without Curly Braces `{}`

```java
// Java program demonstrating do-while loop without curly braces
public class WithoutBraces {
    public static void main(String[] args) {
        int c = 1;
        
        do
            System.out.println("Hello Java!");
        while (c >= 3); // Condition is false, but the loop runs once
    }
}
```

### Output:
```
Hello Java!
```

### Explanation:
Since there is **only one statement** inside the `do` block, curly braces `{}` are optional. The loop executes **once** before checking the condition `(c >= 3)`, which is false.

---

## When to Use do-while Loop?

- When **at least one execution** is required before checking the condition.
- When displaying a **menu-driven system**.
- When handling **user input loops** that must execute at least once.

---

## Summary

| Feature             | while Loop | do-while Loop |
|---------------------|------------|--------------|
| Condition Check     | Before execution | After execution |
| Minimum Executions | **0** (if false initially) | **At least 1** |
| Use Case | When execution depends on a condition | When execution must happen at least once |

The `do-while` loop is a useful construct in Java that ensures at least one execution of the loop body before checking the condition. This is especially beneficial for interactive programs like games, menus, or situations where input validation is required.

---
# Break Statement in Java

## What is the Break Statement?
The `break` statement in Java is used to stop the execution of a loop or a switch case immediately. When a `break` statement is encountered, the control exits the loop or switch case and moves to the next statement after it.

---

## Uses of the Break Statement
1. **Inside a Switch Case** → Stops further case checks once a match is found.
2. **Inside Loops** → Exits a loop when a certain condition is met.
3. **Inside Labeled Blocks** → Exits from nested code blocks.

---

## 1. Break in Switch Case
In a `switch` statement, the `break` statement is used to stop execution after a matching case is found. Without it, all cases after the match will execute.

### Example:
```java
// Java Program to illustrate break in a switch case
class BreakInSwitch {
    public static void main(String[] args) {
        int n = 1;
        
        switch(n) {
            case 1:
                System.out.println("GFG");
                break;
            case 2:
                System.out.println("Second Case");
                break;
            default:
                System.out.println("Default case");
        }
    }
}
```

### Output:
```
GFG
```

### Explanation:
- Since `n = 1`, case `1` executes and prints **GFG**.
- The `break` statement stops further execution, so other cases are skipped.

If there were no `break`, all cases after `1` would run, causing unwanted output.

---

## 2. Break in Loops
The `break` statement can be used inside **for, while,** and **do-while** loops to exit early.

### Example: Using Break in a For Loop
```java
// Java program to illustrate break in a loop
class BreakInLoop {
    public static void main(String[] args) {
        for (int i = 0; i < 10; i++) {
            if (i == 5) {
                break; // Exit loop when i reaches 5
            }
            System.out.println("i: " + i);
        }
        System.out.println("Loop complete.");
    }
}
```

### Output:
```
i: 0
i: 1
i: 2
i: 3
i: 4
Loop complete.
```

### Explanation:
- The loop runs from `0 to 9`.
- When `i == 5`, the `break` statement stops the loop.
- The message **"Loop complete."** is printed after the loop ends.

Without `break`, the loop would have printed numbers from `0 to 9`.

---

## 3. Break in Labeled Blocks
Java allows breaking out of nested code blocks using labels. This is useful for exiting deeply nested structures.

### Example:
```java
// Java program to illustrate break in labeled blocks
class BreakInLabeledBlocks {
    public static void main(String[] args) {
        boolean t = true;

        first: {
            second: {
                third: {
                    System.out.println("Before break statement");
                    if (t) {
                        break second; // Exits the second block
                    }
                    System.out.println("This won't execute.");
                }
                System.out.println("This won't execute.");
            }
            System.out.println("After second block.");
        }
    }
}
```

### Output:
```
Before break statement
After second block.
```

### Explanation:
- The program enters the labeled blocks **first → second → third**.
- When `break second;` is executed, it exits **second** and skips all statements inside it.
- The control jumps to **After second block.**

---

## Summary
| Usage | Purpose |
|--------|--------------------------------|
| **In Loops** | Exits a loop early when a condition is met |
| **In Switch Cases** | Stops further case execution after a match |
| **In Labeled Blocks** | Exits deeply nested code blocks |

### Important Notes:
- `break` **only exits the loop it is inside**, not outer loops.
- `break` in `switch` prevents **fall-through** to other cases.
- `break` in **labeled blocks** allows exiting specific code sections.

---
# Continue Statement in Java

## What is the Continue Statement?
The `continue` statement in Java is used inside loops like `for`, `while`, and `do-while`. When encountered, it skips the rest of the current iteration and moves to the next iteration of the loop.

---

## Uses of the Continue Statement
1. **Inside For Loop** → Skips an iteration and moves to the update statement.
2. **Inside While Loop** → Skips an iteration and moves to the Boolean condition.
3. **Inside Do-While Loop** → Skips an iteration but ensures the loop executes at least once.
4. **Inside Nested Loops** → Skips the current iteration in the inner loop.

---

## 1. Continue in For Loop

### Example:
```java
// Java Program to illustrate continue in a for loop
class ContinueInForLoop {
    public static void main(String[] args) {
        for (int i = 0; i <= 5; i++) {
            if (i == 3) {
                continue; // Skip iteration when i == 3
            }
            System.out.print(i + " ");
        }
    }
}
```

### Output:
```
0 1 2 4 5
```

### Explanation:
- The loop runs from `0 to 5`.
- When `i == 3`, `continue` is executed, skipping the print statement.
- The loop continues with the next iteration.

---

## 2. Continue in While Loop

### Example:
```java
// Java Program to illustrate continue in a while loop
class ContinueInWhileLoop {
    public static void main(String[] args) {
        int c = 0;
        while (c <= 5) {
            if (c == 3) {
                c++;
                continue;
            }
            System.out.print(c + " ");
            c++;
        }
    }
}
```

### Output:
```
0 1 2 4 5
```

### Explanation:
- When `c == 3`, the `continue` statement skips printing `3`.
- The loop moves to the next iteration.

---

## 3. Continue in Do-While Loop

### Example:
```java
// Java Program to illustrate continue in a do-while loop
class ContinueInDoWhileLoop {
    public static void main(String[] args) {
        int i = 0;
        do {
            if (i == 3) {
                i++;
                continue;
            }
            System.out.print(i + " ");
            i++;
        } while (i <= 5);
    }
}
```

### Output:
```
0 1 2 4 5
```

### Explanation:
- When `i == 3`, the `continue` statement skips printing `3`.
- The loop proceeds with the next iteration.

---

## 4. Continue in Nested Loops

### Example:
```java
// Java Program to illustrate continue in nested loops
class ContinueInNestedLoops {
    public static void main(String[] args) {
        for (int i = 1; i <= 4; i++) {
            for (int j = 1; j <= 3; j++) {
                if (i == 3 && j == 2) {
                    continue;
                }
                System.out.print(i + "." + j + "  ");
            }
            System.out.println();
        }
    }
}
```

### Output:
```
1.1  1.2  1.3  
2.1  2.2  2.3  
3.1  3.3  
4.1  4.2  4.3  
```

### Explanation:
- When `i == 3` and `j == 2`, the `continue` statement skips that iteration.
- The rest of the iterations execute normally.

---

## 5. Using Break and Continue Together

### Example:
```java
// Java Program to illustrate both break and continue
class BreakAndContinue {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            if (i == 3) {
                continue; // Skip iteration when i == 3
            }
            if (i == 7) {
                break; // Exit loop when i == 7
            }
            System.out.print(i + " ");
        }
    }
}
```

### Output:
```
1 2 4 5 6
```

### Explanation:
- `continue` skips printing `3`.
- `break` stops the loop completely when `i == 7`.

---

## Summary
| Statement | Purpose |
|-----------|---------------------------------|
| **Break** | Exits a loop or switch case completely |
| **Continue** | Skips the current iteration and proceeds with the next |

### Important Notes:
- `continue` **only skips the current iteration**, the loop continues.
- `continue` in a `for` loop moves control to the **update statement**.
- `continue` in a `while` or `do-while` loop moves control to the **Boolean condition**.

---
# Java `return` Keyword

_Last Updated: 02 Jan, 2025_

The `return` keyword in Java is a reserved keyword used to exit from a method, with or without a value. It helps in returning a value from a method or simply stopping the method execution.

## Categories of `return` Usage
There are two main cases where the `return` keyword is used:
1. **Methods Returning a Value**
2. **Methods Not Returning a Value**

## 1. Methods Returning a Value
If a method has a return type (like `int`, `double`, `String`, etc.), the `return` statement must be followed by a value of that type.

### Example: Returning a Value
```java
// Java Program to Illustrate Usage of return Keyword
class Geeks {
    // Method to calculate average
    double avg(double x, double y) {
        double res = (x + y) / 2.0;
        return res; // Return the calculated result
    }

    public static void main(String[] args) {
        System.out.println(new Geeks().avg(5.5, 6.5));
    }
}
```
**Output:**
```
6.0
```
**Explanation:** The `avg` method calculates the average and returns the result, which is printed in the `main` method.

## 2. Methods Not Returning a Value
For methods that do not return a value (i.e., methods with `void` return type), the `return` statement can be either omitted or used alone to exit the method early.

### Example 1: Method Without `return`
```java
// Java program to illustrate no return keyword needed in void method
class Geeks {
    void calc(int a, int b) {
        int res = (a + b) / 10;
        System.out.println(res);
    }

    public static void main(String[] args) {
        new Geeks().calc(5, 5);
        System.out.println("No return keyword is used, and program executed successfully");
    }
}
```
**Output:**
```
1
No return keyword is used, and program executed successfully
```

### Example 2: Using `return` in `void` Method
```java
// Java program to illustrate usage of return keyword in void method
class Geeks {
    void check(double v) {
        if (v < 9) {
            return; // Exit method if condition is met
        }
        v++;
    }

    public static void main(String[] args) {
        Geeks o = new Geeks();
        o.check(5.5);
        System.out.println("Program executed successfully");
    }
}
```
**Output:**
```
Program executed successfully
```
**Explanation:** When `v < 9`, the method exits before executing the next statement.

---

## `return` Statement at the End of a Method
The `return` statement can be used anywhere in the method but must be the last statement executed.

### Example: Return at Different Places
```java
// Java program to illustrate return is not always the last statement
class Geeks {
    void demoFunc(double n) {
        if (n < 9) return; // Exit if condition is met
        n++;
    }

    public static void main(String[] args) {
        new Geeks().demoFunc(7);
        System.out.println("Program executed successfully");
    }
}
```
**Output:**
```
Program executed successfully
```

---

## Unreachable Code and Compile-Time Error
If any statement is placed after `return`, it causes a **compile-time error** because the code after `return` is unreachable.

### Example: Unreachable Code
```java
// Java program to illustrate unreachable statement error
public class Geeks {
    void demoFunc(double j) {
        return;
        ++j; // This line will cause a compile-time error
    }

    public static void main(String[] args) {
        new Geeks().demoFunc(5);
    }
}
```
**Error:** `Unreachable statement`

---

## Using `return` Inside a Condition
The `return` statement can be used inside an `if` condition to exit early.

### Example: Returning Inside an `if` Statement
```java
// Java program to illustrate usage of return keyword
class Geeks {
    void demo(double v) {
        if (v < 0) {
            System.out.println(v);
            return; // Exit method early
        } else {
            ++v;
        }
    }

    public static void main(String[] args) {
        new Geeks().demo(-1);
        System.out.println("Program executed successfully");
    }
}
```
**Output:**
```
-1.0
Program executed successfully
```
**Explanation:** If `v < 0`, the method exits early, and `++v` is not executed.

---

## Summary
- `return` is used to exit a method, optionally returning a value.
- In non-`void` methods, it must return a value matching the return type.
- In `void` methods, `return` can be used to exit early but doesn’t return a value.
- A statement after `return` causes a compile-time error.
- `return` is often used inside conditions to stop execution early.

---
## Difference Between `for` Loop and `while` Loop in Java

| Feature           | `for` Loop | `while` Loop |
|------------------|-----------|-------------|
| **Usage** | Used when the number of iterations is known beforehand. | Used when the number of iterations is not known beforehand and depends on a condition. |
| **Structure** | Includes initialization, condition, and update in a single line. | Only includes the condition; initialization and update must be handled separately. |
| **Syntax** | ```java
for(initialization; condition; update) {
    // loop body
}
``` | ```java
initialization;
while(condition) {
    // loop body
    update;
}
``` |
| **Execution Flow** | 1. Initialization → Condition Check → Execution → Update → Repeat until condition fails. | 1. Initialization → Condition Check → Execution → Update → Repeat until condition fails. |
| **Best Use Case** | When you know the exact number of times the loop should run. | When the loop should run until a certain condition is met, but the number of iterations is unknown. |
| **Example** | ```java
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}
``` | ```java
int i = 0;
while (i < 5) {
    System.out.println(i);
    i++;
}
``` |
| **Readability** | More compact and structured. | More flexible but requires careful handling of initialization and update. |
| **Use in Infinite Loop** | ```java
for(;;) {
    // Infinite loop
}
``` | ```java
while(true) {
    // Infinite loop
}
``` |
| **Flexibility** | Less flexible since all parts of the loop are in a single line. | More flexible as initialization and update can be placed anywhere. |

## Summary
- Use `for` loop when the number of iterations is fixed.
- Use `while` loop when the loop depends on a condition that may change dynamically.
---
### Java Methods

Java Methods are blocks of code that perform a specific task. A method allows us to reuse code, improving both efficiency and organization. All methods in Java must belong to a class. Methods are similar to functions and expose the behavior of objects.

#### Example:

```java
// Creating a method that prints a message
public class Method {
    
    // Method to print message
    public void printMessage() {
        System.out.println("Hello, Geeks!");
    }

    public static void main(String[] args) {
        // Create an instance of the Method class
        Method m = new Method();
        m.printMessage();  // Calling the method
    }
}
```

**Output:**
```
Hello, Geeks!
```

### Syntax of a Method
```java
<access_modifier> <return_type> <method_name>(list_of_parameters) {
    // body
}
```

### Key Components of a Method Declaration

- **Modifier:** Specifies the method’s access level (e.g., public, private, protected, or default).
- **Return Type:** The type of value returned, or void if no value is returned.
- **Method Name:** Follows Java naming conventions; it should start with a lowercase verb and use camel case for multiple words.
- **Parameters:** A list of input values (optional). Empty parentheses are used if no parameters are needed.
- **Exception List:** The exceptions the method might throw (optional).
- **Method Body:** Contains the logic to be executed (optional for abstract methods).

### Types of Methods in Java

#### 1. Predefined Method
Predefined methods are already defined in the Java class libraries. They are also known as standard library methods or built-in methods.

**Example:**
```java
Math.random();    // returns a random value
Math.PI;         // returns pi value
```

#### 2. User-defined Method
User-defined methods are created by the programmer and can be modified as per requirements.

**Example:**
```java
void sayHello() {
    System.out.println("Hello!");
}
```

### Different Ways to Create Java Methods

#### 1. Instance Method
Access instance data using an object name. Declared inside a class.

```java
// Instance Method
void methodName() {
    // instance method body
}
```

#### 2. Static Method
Access static data using a class name. Declared inside a class with the `static` keyword.

```java
// Static Method
static void methodName() {
    // static method body
}
```

### Method Signature
The method signature consists of:
- Number of parameters
- Type of parameters
- Order of parameters

```java
max(int x, int y) // Number of parameters: 2, Type: int
```

### Naming a Method
**Rules:**
- Method names should start with a lowercase verb.
- If a method has multiple words, the first word must be a verb, followed by an adjective or noun.
- In multi-word method names, capitalize the first letter of each word except the first.
- Methods in the same class can have the same name (method overloading is allowed).

### Method Calling
Methods allow code reuse and better organization. A method must be called to execute its functionality.

A method returns to the code that invoked it when:
- It completes all the statements in the method.
- It reaches a return statement.
- It throws an exception.

#### Example 1: Method Calling Using an Object

```java
class Add {
    int s = 0;
    public int addTwoInt(int a, int b) {
        s = a + b;
        return s;
    }
}

class Main {
    public static void main(String[] args) {
        Add a = new Add();
        int res = a.addTwoInt(1, 2);
        System.out.println("Sum: " + res);  
    }
}
```

**Output:**
```
Sum: 3
```

### Passing Parameters to a Method
Sometimes, we may not know the number of parameters to be passed. Java provides ways to handle such cases:

- Passing an **Array** as an Argument
- Passing **Variable-arguments** as an Argument
- **Method Overloading**

### Memory Allocation for Method Calls
Method calls are implemented using a stack. Whenever a method is called, a **stack frame** is created in the stack memory. This frame stores:
- Arguments passed
- Local variables
- Return values

Once execution completes, the allocated stack frame is removed.

### Example: Accessor and Mutator Methods

```java
public class Geeks {
    private int num;
    private String n;

    // Accessor (getter) methods
    public int getNumber() { 
        return num; 
    }
    public String getName() { 
        return n; 
    }

    // Mutator (setter) methods
    public void setNumber(int num) { 
        this.num = num; 
    }
    public void setName(String n) { 
        this.n = n; 
    }

    // Other methods
    public void printDetails() {
        System.out.println("Number: " + num);
        System.out.println("Name: " + n);
    }

    // Main method to run the code
    public static void main(String[] args) {
        Geeks g = new Geeks();
        g.setNumber(123);   // Set the number
        g.setName("GFG Write");   // Set the name
        g.printDetails();  
    }
}
```

**Output:**
```
Number: 123
Name: GFG Write
```

### Advantages of Methods
- **Reusability:** Write once, use multiple times.
- **Abstraction:** Hide complex logic.
- **Encapsulation:** Encapsulate logic and data.
- **Modularity:** Organize code into smaller, manageable units.
- **Customization:** Easily modify for specific tasks.
- **Improved Performance:** Efficiently structured methods improve performance.

### FAQs

**Q: What is a method in Java programming?**
A method is a collection of statements that perform a specific task and return a result to the caller.

**Q: What are the parts of a method in Java?**
- Modifiers
- Return Type
- Method Name
- Parameters
- Method Body

**Q: Does Java support method overloading?**
Yes, Java supports method overloading by changing the parameter list.

**Q: What are the types of methods in Java?**
1. **Instance methods**
2. **Static methods**

**Q: What is the difference between a Constructor and a Method in Java?**
A **method** is a block of code that performs certain tasks, whereas a **constructor** is a special type of method used to initialize objects when they are created. Constructors have the same name as the class.

---
### Java Methods

Java Methods are blocks of code that perform a specific task. A method allows us to reuse code, improving both efficiency and organization. All methods in Java must belong to a class. Methods are similar to functions and expose the behavior of objects.

#### Example:

```java
// Creating a method
// that prints a message
public class Method {
  
    // Method to print message
    public void printMessage() {
        System.out.println("Hello, Geeks!");
    }

    public static void main(String[] args) {
      
        // Create an instance of the Method class
        Method m = new Method();
        m.printMessage();  // Calling the method
    }
}
```

**Output:**
```
Hello, Geeks!
```

### Syntax of a Method

```java
<access_modifier> <return_type> <method_name>( list_of_parameters) {
    // body
}
```

### Key Components of a Method Declaration
- **Modifier:** Specifies the method’s access level (e.g., public, private, protected, or default).
- **Return Type:** The type of value returned, or `void` if no value is returned.
- **Method Name:** Should start with a lowercase verb and use camel case for multiple words.
- **Parameters:** List of input values (optional).
- **Exception List:** The exceptions the method might throw (optional).
- **Method Body:** Contains the logic to be executed.

---

### Types of Methods in Java

#### 1. Predefined Method
Predefined methods are the methods already defined in the Java class libraries.

**Example:**
```java
Math.random();  // returns a random value
Math.PI;       // returns pi value
```

#### 2. User-defined Method
Methods written by the user or programmer.

**Example:**
```java
void sayHello() {
    System.out.println("Hello!");
}
```

---

### Calling a Method in Java
Calling a method allows reusing code and organizing our program effectively.

#### Example:
```java
class GFG {
  
    // User-defined method
    void hello() {
        System.out.println("This is a user-defined method.");
    }
    public static void main(String[] args) {
      
        // Create an object
        GFG obj = new GFG(); 
      
        // Call the method
        obj.hello();          
    }
}
```

**Output:**
```
This is a user-defined method.
```

> **Note:** User-Defined non-static methods can be accessed only using an instance of the class.

---

### 1. Calling the Abstract Methods
Abstract methods are declared in abstract classes. They must be implemented in subclasses.

**Example:**
```java
// Java Program to call Abstract Methods
abstract class GFGhelp {
    // Creating abstract method
    abstract void check(String n);
}

public class GFG extends GFGhelp {
    public static void main(String[] args) {
        // Creating the instance of the class
        GFG ob = new GFG();
        // Accessing the abstract method
        ob.check("GFG");
    }
    
    @Override 
    void check(String n) {
        System.out.println(n);
    }
}
```

**Output:**
```
GFG
```

---

### 2. Calling the Predefined Methods
These methods are provided by Java’s standard library, such as `hashCode()` from the `Object` class.

**Example:**
```java
// Java Program to call Predefined Methods
public class GFG {
    public static void main(String[] args) {
        // Creating object of the class
        GFG ob = new GFG();
        // Calling predefined method
        System.out.println(ob.hashCode());
    }
}
```

**Output:** _(varies)_
```
1510467688
```

---

### 3. Calling the Static Methods
Static methods belong to the class and can be called without creating an object.

**Example:**
```java
// Java Program to call Static Methods
class Test {
    // Static method
    static void hello() {
        System.out.println("Hello");
    }
}

class GFG {
    public static void main(String[] args) {
        // Calling the static Method
        Test.hello();
    }
}
```

**Output:**
```
Hello
```

> **Explanation:** We call a static method `hello()` from the `Test` class without creating an instance.

---

### Advantages of Methods
- **Reusability:** Write code once and use it many times.
- **Abstraction:** Hide complex logic and provide a simple interface.
- **Encapsulation:** Protect complex logic and data.
- **Modularity:** Organize code into smaller, manageable units.
- **Customization:** Easily modified for specific tasks.
- **Improved Performance:** Enhances code efficiency.

---

### FAQs

**1. What is a method in Java programming?**
Java Method is a collection of statements that perform a specific task and return a result.

**2. What are the parts of a method in Java?**
- Modifiers
- Return Type
- Method Name
- Parameters
- Method Body

**3. Does Java support method overloading?**
Yes, Java supports method overloading by changing the parameters or return type.

**4. What are the types of methods in Java?**
- Instance methods
- Static methods

**5. What is the main difference between Constructor and Method in Java?**
A method is a block of code performing tasks, whereas a constructor initializes objects when created and has the same name as the class.

---
### Static Method vs Instance Method in Java  
*Last Updated: 02 Jan, 2025*  

In Java, methods are mainly divided into two parts based on how they are associated with a class:

1. **Static Method:** Belongs to the class and can be called without creating an object.
2. **Instance Method:** Belongs to an object and requires an object to be called.

### Static Method vs Instance Method (Comparison Table)

| **Feature**       | **Static Method** | **Instance Method** |
|-------------------|------------------|---------------------|
| **Definition**    | Created using the `static` keyword and retrieved without creating an object. | Requires an object of its class to be invoked. |
| **Access**       | Can access only static variables and methods. | Can access both static and instance members. |
| **`this` keyword** | Cannot use `this` keyword within static methods. | Can use `this` to refer to the current object. |
| **Override**      | Does not support runtime polymorphism. | Supports runtime polymorphism. |

---

## Static Method  
A static method is created using the `static` keyword. It can be called without creating an object of the class, referenced by the class name itself or a reference to an object of that class.

### **Memory Allocation of Static Methods:**  
- Static methods belong to the class, not its objects.
- They are stored in the **Permanent Generation (PermGen)** space (until Java 7) or **Metaspace** (from Java 8 onwards).
- Local variables and arguments of static methods are stored in the **stack**.

### **Important Points:**  
✔ Static methods are shared among all objects of the class.  
✔ They cannot be overridden (they use **static binding** at compile time).  
✔ If a superclass and subclass have static methods with the same name, it results in **Method Hiding**.

### **Example:**
```java
// Demonstration of static method  
class Geeks {
  // Static method 
  public static void greet(){
    System.out.println("Hello Geek!");
  }

  public static void main (String[] args) {
    // Calling the method directly
    greet();
    
    // Calling the method using the class name
    Geeks.greet();  
  }
}
```
**Output:**  
```
Hello Geek!
Hello Geek!
```

---

## Instance Method  
Instance methods require an object of their class to be created before they can be called.

### **Memory Allocation of Instance Method:**  
- Instance methods are stored in **Permanent Generation space** (till Java 7) and **Metaspace** (from Java 8).
- Their parameters, local variables, and return values are stored in the **stack**.
- They can be called within their class or from other classes, based on their access modifiers.

### **Important Points:**  
✔ Instance methods belong to an object, not the class.  
✔ They are stored in one memory location and identify their object through the `this` pointer.  
✔ They can be overridden as they use **dynamic binding** at runtime.

### **Example:**
```java
// Demonstrating the use of an instance method
class Test {
    String n = "";

    // Instance method 
    public void test(String n) { 
      this.n = n; 
    }
}

class Geeks {
    public static void main(String[] args) {
        // Creating an instance of the class
        Test t = new Test();

        // Calling an instance method 
        t.test("GeeksforGeeks");
        System.out.println(t.n);
    }
}
```
**Output:**  
```
GeeksforGeeks
```

---

## **FAQs**

### **1. What if a static variable refers to an Object?**
```java
static int i = 1; 
static Object obj = new Object();
```
✔ Value of `i`: Stored in **Metaspace** (PermGen in Java 7 and earlier).  
✔ Reference `obj`: Stored in **Metaspace**, but the object it refers to is stored in the **heap**.

### **2. When should we use static methods?**
Use static methods when:
✔ The method does **not depend on the state** of an object.  
✔ The code needs to be **shared** across all objects of a class (e.g., utility methods like `Math.sqrt()`).  

### **3. Can we call a static method directly without creating an object?**
Yes! Static methods can be called:
✔ **Directly** (if within the same class).  
✔ Using the **class name** (if in a different class).  

### **4. How to decide whether to use a static or instance method?**
✔ Use **static methods** for **class-level** operations or utilities.  
✔ Use **instance methods** for operations that depend on the state of an **object**.  

---

### **Conclusion**  
- **Static methods** belong to the class and do not require object instantiation.  
- **Instance methods** belong to an object and need an object to be called.  
- Use static methods for utility functions and instance methods for object-specific behavior.

---
# Access Modifiers in Java

**Last Updated:** 15 Dec, 2024  

In Java, access modifiers help restrict the scope of a class, constructor, variable, method, or data member. They provide security and control accessibility depending on the modifier used. This article covers Java Access Modifiers, their types, and their uses.

## Types of Access Modifiers
There are **four** types of access modifiers in Java:

1. **Default** – No keyword required
2. **Private**
3. **Protected**
4. **Public**

## 1. Default Access Modifier
If no access modifier is specified for a class, method, or data member, it has the default access modifier. This means they are accessible **only within the same package**.

### Example 1: Accessing Default Modifier Within the Same Package
```java
// Package p1
package p1;

// Default access modifier
class Geek {
    void display() {
        System.out.println("Hello World!");
    }
}
```

### Example 2: Error When Accessing Default Modifier Across Packages
```java
// Package p2
package p2;
import p1.*;    // Importing package p1

class GeekNew {
    public static void main(String args[]) {
        Geek o = new Geek(); // Error: Geek is not public
        o.display(); // Not accessible outside package
    }
}
```

## 2. Private Access Modifier
The `private` access modifier is specified using the `private` keyword. 
- It allows access **only within the class**.
- Other classes, even within the same package, **cannot** access private members.
- **Top-level classes cannot be declared as private**.

### Example: Trying to Access a Private Method (Compile-time Error)
```java
// Package p1
package p1;

class A {
    private void display() {
        System.out.println("GeeksforGeeks");
    }
}

class B {
    public static void main(String args[]) {
        A obj = new A();
        obj.display(); // Compile-time error
    }
}
```

## 3. Protected Access Modifier
The `protected` access modifier allows access **within the same package** and **by subclasses in different packages**.

### Example 1: Accessing Protected Modifier Within the Same Package
```java
// Package p1
package p1;

public class A {
    protected void display() {
        System.out.println("GeeksforGeeks");
    }
}
```

### Example 2: Accessing Protected Modifier in a Subclass Across Packages
```java
// Package p2
package p2;
import p1.*; // Importing package p1

class B extends A {
    public static void main(String args[]) {
        B obj = new B();
        obj.display(); // Accessible via inheritance
    }
}
```

## 4. Public Access Modifier
The `public` access modifier allows access **from anywhere in the program**. 
- It has **the widest scope** among all access modifiers.
- There is **no restriction** on its access.

### Example 1: Public Method Accessible Within the Same Package
```java
// Package p1
package p1;

public class A {
    public void display() {
        System.out.println("GeeksforGeeks");
    }
}
```

### Example 2: Public Method Accessible Across Packages
```java
// Package p2
package p2;
import p1.*;

class B {
    public static void main(String args[]) {
        A obj = new A();
        obj.display(); // No restrictions
    }
}
```

## Comparison Table of Access Modifiers in Java

| Feature        | Default | Private | Protected | Public |
|---------------|---------|---------|-----------|--------|
| **Accessible within same class** | ✅ | ✅ | ✅ | ✅ |
| **Accessible within same package** | ✅ | ❌ | ✅ | ✅ |
| **Accessible in subclasses (other package)** | ❌ | ❌ | ✅ | ✅ |
| **Accessible from anywhere** | ❌ | ❌ | ❌ | ✅ |

## When to Use Access Modifiers?

### Algorithm to Use Access Modifiers in Java
1. **Define a class**: Create a class for the required object.
2. **Define instance variables**: Define the necessary attributes.
3. **Set an access modifier**:
   - Use `private` for variables that should be hidden.
   - Use `protected` for variables accessible in subclasses.
   - Use `public` for variables that should be accessible from anywhere.
4. **Use getter and setter methods**: Control access even for public variables to maintain encapsulation.

## FAQs – Access Modifiers in Java

### What are access modifiers in Java?
Access modifiers are keywords used to control the accessibility of classes, methods, and variables.

### What is the default access modifier in Java?
The default access modifier allows access only **within the same package**.

### What are the 12 modifiers in Java?
The 12 Java modifiers are:
`public`, `private`, `protected`, `default`, `static`, `final`, `synchronized`, `abstract`, `native`, `strictfp`, `transient`, and `volatile`.

### Can a private method be accessed outside its class?
No, a `private` method **cannot** be accessed outside its class.

### What does the protected access modifier do?
A `protected` modifier allows access **within the same package** and **by subclasses in different packages**.

### Can public variables be accessed from any class?
Yes, `public` variables are accessible **from any class**, regardless of the package.

---
# Command Line Arguments in Java

Java command-line argument is an argument passed at the time of running the Java program. These arguments are passed from the console and can be received in the Java program as input. The users can pass arguments during execution by specifying them after the program name.

## How Command Line Arguments Work

- The arguments are passed as **space-separated** values.
- They are **stored in a String array (`args[]`)** provided to the `main()` method.
- Java **automatically converts** these arguments into strings.
- The arguments can be **accessed using their index positions** (`args[0]`, `args[1]`, etc.).

## Example 1: Printing the First Argument

```java
// Java Program to Illustrate First Argument
class GFG {
    public static void main(String[] args) {
        // Printing the first argument
        System.out.println(args[0]);
    }
}
```

### **Output**

#### **Command:**
```sh
java GFG GeeksForGeeks
```

#### **Output:**
```
GeeksForGeeks
```

#### **Explanation:**
- If we run the Java program with `java GFG GeeksForGeeks`, `args[0]` will contain `GeeksForGeeks`.
- If no arguments are provided (e.g., just `java GFG`), it will throw an `ArrayIndexOutOfBoundsException` because the `args` array is empty.

---

## Example 2: Displaying All Command Line Arguments

```java
// Java Program to Check for Command Line Arguments
class Hello {
    public static void main(String[] args) {
        // Checking if length of args array is greater than 0
        if (args.length > 0) {
            System.out.println("The command line arguments are:");
            
            // Iterating over the args array
            for (String val : args)
                System.out.println(val);
        } else {
            System.out.println("No command line arguments found.");
        }
    }
}
```

### **Output**

#### **Command:**
```sh
java Hello Geeks at GeeksforGeeks
```

#### **Output:**
```
The command line arguments are:
Geeks
at
GeeksforGeeks
```

#### **Explanation:**
- The program checks whether any command-line arguments were passed.
- If arguments exist, they are displayed one by one.
- If no arguments are passed, it prints `No command line arguments found.`

---

## Steps to Compile and Run a Java Program with Command Line Arguments

1. Save the program as `Hello.java`
2. Open the **command prompt** and navigate to the file location.
3. Compile the program:
   ```sh
   javac Hello.java
   ```
4. Run the program with arguments:
   ```sh
   java Hello Geeks at GeeksforGeeks
   ```
5. Press **Enter** and observe the output.

---

## Important Points

| Feature | Description |
|---------|-------------|
| **String Input** | Command-line arguments are space-separated strings. |
| **Dynamic Input** | Allows users to pass different values dynamically. |
| **Length Check** | The number of arguments can be checked using `args.length`. |
| **Indexes** | Access specific arguments using `args[0]`, `args[1]`, etc. |

### **Example of Checking Argument Length**

```java
class Test {
    public static void main(String[] args) {
        System.out.println("Number of arguments: " + args.length);
    }
}
```

#### **Command:**
```sh
java Test 1 2 3 4
```

#### **Output:**
```
Number of arguments: 4
```

### **Handling Integer Arguments**

Since command-line arguments are treated as **Strings**, they must be converted to numbers before performing mathematical operations.

```java
class Sum {
    public static void main(String[] args) {
        int num1 = Integer.parseInt(args[0]); // Convert first argument to int
        int num2 = Integer.parseInt(args[1]); // Convert second argument to int
        int sum = num1 + num2;
        System.out.println("Sum: " + sum);
    }
}
```

#### **Command:**
```sh
java Sum 10 20
```

#### **Output:**
```
Sum: 30
```

---

## Conclusion
- Command-line arguments **provide dynamic input** to Java programs.
- They are stored in the **`args[]` array** as strings.
- **They must be converted** when working with numerical values.
- **Always check the length** of `args[]` to avoid errors.

---
# Variable Arguments (Varargs) in Java

## Introduction
Variable Arguments (Varargs) in Java allow a method to accept a variable number of arguments. This feature simplifies the creation of methods that need to take multiple parameters without overloading methods.

## Syntax of Varargs
```java
public static void methodName(datatype... varName) {
    // method body
}
```
- The three dots `...` indicate that the method can accept multiple arguments of the specified datatype.
- Internally, Varargs are treated as an array.

## Example: Using Varargs in Java
```java
class Geeks {
    public static void Names(String... n) {
        for (String i : n) {
            System.out.print(i + " ");
        }
        System.out.println();
    }

    public static void main(String[] args) {
        Names("geek1", "geek2");           
        Names("geek1", "geek2", "geek3");   
    }
}
```
### Output:
```
geek1 geek2 
geek1 geek2 geek3 
```
### Explanation:
- The `Names(String... n)` method accepts multiple `String` arguments.
- A for-each loop iterates through the `n` array and prints each name.

## Need for Varargs
Before JDK 5, variable-length arguments were handled in two ways:
1. **Method Overloading** - Creating multiple overloaded methods for different argument numbers.
2. **Using Arrays** - Passing an array to hold multiple arguments.

Both approaches increased code complexity and reduced readability. Java 5 introduced Varargs to simplify this process.

## Example 1: Varargs with Integer Arguments
```java
class Test1 {
    static void fun(int... a) {
        System.out.println("Number of arguments: " + a.length);
        for (int i : a)
            System.out.print(i + " ");
        System.out.println();
    }

    public static void main(String args[]) {
        fun(100);
        fun(1, 2, 3, 4);
        fun();
    }
}
```
### Output:
```
Number of arguments: 1
100 
Number of arguments: 4
1 2 3 4 
Number of arguments: 0
```

## Using Varargs with Other Parameters
A method can have both normal parameters and a variable argument, but the Varargs parameter **must be the last parameter**.

### Example 2: Varargs with Other Arguments
```java
class Test2 {
    static void fun2(String s, int... a) {
        System.out.println("String: " + s);
        System.out.println("Number of arguments: " + a.length);
        for (int i : a)
            System.out.print(i + " ");
        System.out.println();
    }

    public static void main(String args[]) {
        fun2("GeeksforGeeks", 100, 200);
        fun2("CSPortal", 1, 2, 3, 4, 5);
        fun2("forGeeks");
    }
}
```
### Output:
```
String: GeeksforGeeks
Number of arguments is: 2
100 200 
String: CSPortal
Number of arguments is: 5
1 2 3 4 5 
String: forGeeks
Number of arguments is: 0
```

## Erroneous Varargs Usage
### Case 1: Multiple Varargs in One Method
```java
void method(String... gfg, int... q) { }
```
**Error:** Only one Varargs parameter is allowed per method.

### Case 2: Varargs as First Parameter
```java
void method(int... gfg, String q) { }
```
**Error:** Varargs should be the last parameter in the method.

## Important Points
- Varargs methods can be **overloaded**, but it may cause ambiguity.
- Before JDK 5, handling variable-length arguments required **method overloading** or **array arguments**.
- A method **can have only one Varargs parameter**.
- The **Varargs parameter must always be the last parameter**.

---

# Java Arrays - A Complete Guide

## What is an Array in Java?
An **array** is a collection of similar types of elements stored in contiguous memory locations. In Java, arrays are **fixed in size** and can store **primitives** (int, char, etc.) or **objects**.

## Declaring an Array
Arrays in Java are declared using the following syntax:

```java
// Syntax:
dataType[] arrayName;
```

### Example:
```java
int[] numbers; // Declares an array of integers
String[] names; // Declares an array of strings
```

## Initializing an Array
There are multiple ways to initialize an array in Java:

### 1. Using `new` keyword
```java
int[] numbers = new int[5]; // Creates an array of size 5 with default values (0)
```

### 2. Using an Array Literal
```java
int[] numbers = {1, 2, 3, 4, 5};
```

### 3. Dynamic Initialization
```java
int size = 4;
int[] numbers = new int[size]; // Creates an array of size 4
```

## Accessing Array Elements
Each element in an array is accessed using an **index** (starting from `0`).

```java
int[] numbers = {10, 20, 30, 40};
System.out.println(numbers[0]); // Output: 10
System.out.println(numbers[2]); // Output: 30
```

## Modifying Array Elements
```java
int[] numbers = {5, 10, 15};
numbers[1] = 50; // Changing the second element
System.out.println(numbers[1]); // Output: 50
```

## Array Length
The length of an array is determined using the `.length` property.

```java
int[] numbers = {1, 2, 3, 4};
System.out.println(numbers.length); // Output: 4
```

## Looping Through an Array

### 1. Using a `for` loop
```java
int[] numbers = {10, 20, 30, 40};
for (int i = 0; i < numbers.length; i++) {
    System.out.println(numbers[i]);
}
```

### 2. Using an Enhanced `for` loop (for-each)
```java
for (int num : numbers) {
    System.out.println(num);
}
```

## Multi-Dimensional Arrays
Java supports **multi-dimensional arrays**, commonly used for matrices.

### Declaring and Initializing a 2D Array
```java
int[][] matrix = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
};
```

### Accessing Elements in a 2D Array
```java
System.out.println(matrix[1][2]); // Output: 6
```

### Looping Through a 2D Array
```java
for (int i = 0; i < matrix.length; i++) {
    for (int j = 0; j < matrix[i].length; j++) {
        System.out.print(matrix[i][j] + " ");
    }
    System.out.println();
}
```

## Array Methods in Java
Java provides various utility methods in `java.util.Arrays` class.

### 1. Sorting an Array
```java
import java.util.Arrays;
int[] numbers = {5, 2, 8, 1, 3};
Arrays.sort(numbers);
System.out.println(Arrays.toString(numbers)); // Output: [1, 2, 3, 5, 8]
```

### 2. Filling an Array
```java
Arrays.fill(numbers, 7);
System.out.println(Arrays.toString(numbers)); // Output: [7, 7, 7, 7, 7]
```

### 3. Copying an Array
```java
int[] newArray = Arrays.copyOf(numbers, numbers.length);
System.out.println(Arrays.toString(newArray));
```

### 4. Comparing Arrays
```java
int[] arr1 = {1, 2, 3};
int[] arr2 = {1, 2, 3};
System.out.println(Arrays.equals(arr1, arr2)); // Output: true
```

## Limitations of Java Arrays
- **Fixed Size**: Cannot be resized once created.
- **Only Stores Homogeneous Data**: Cannot store different data types in the same array.
- **No Built-in Methods for Insertion/Deletion**: Unlike Lists.

## Alternative to Arrays
Use **ArrayList** from `java.util` package for a dynamic array.
```java
import java.util.ArrayList;
ArrayList<Integer> list = new ArrayList<>();
list.add(10);
list.add(20);
System.out.println(list); // Output: [10, 20]
```

## Conclusion
Java arrays are fundamental data structures for storing multiple values efficiently. Understanding how to declare, initialize, and manipulate arrays is crucial for Java programming.
---
# Jagged Arrays, Arrays Class, and Final Arrays

## 1. Jagged Arrays in Java
Jagged arrays are multi-dimensional arrays where each row can have a different number of columns.

### Declaration and Initialization:
```java
public class JaggedArrayExample {
    public static void main(String[] args) {
        // Declare a 2D Jagged Array
        int[][] jaggedArray = new int[3][]; 
        
        // Initialize rows with different sizes
        jaggedArray[0] = new int[2]; // 2 elements in row 0
        jaggedArray[1] = new int[4]; // 4 elements in row 1
        jaggedArray[2] = new int[3]; // 3 elements in row 2

        // Assign values
        jaggedArray[0][0] = 1;
        jaggedArray[0][1] = 2;
        jaggedArray[1][0] = 3;
        jaggedArray[1][1] = 4;
        jaggedArray[1][2] = 5;
        jaggedArray[1][3] = 6;
        jaggedArray[2][0] = 7;
        jaggedArray[2][1] = 8;
        jaggedArray[2][2] = 9;

        // Print Jagged Array
        for (int i = 0; i < jaggedArray.length; i++) {
            for (int j = 0; j < jaggedArray[i].length; j++) {
                System.out.print(jaggedArray[i][j] + " ");
            }
            System.out.println();
        }
    }
}
```
### Output:
```
1 2 
3 4 5 6 
7 8 9 
```

---

## 2. Arrays Class in Java
Java provides the `Arrays` class in `java.util` package for performing various operations on arrays.

### Common Methods of Arrays Class:

#### 1. Sorting an Array (`Arrays.sort()`)
```java
import java.util.Arrays;
public class ArraysSortExample {
    public static void main(String[] args) {
        int[] arr = {5, 2, 8, 3, 1};
        Arrays.sort(arr);
        System.out.println(Arrays.toString(arr)); // [1, 2, 3, 5, 8]
    }
}
```

#### 2. Binary Search (`Arrays.binarySearch()`)
```java
import java.util.Arrays;
public class ArraysBinarySearch {
    public static void main(String[] args) {
        int[] arr = {1, 2, 3, 5, 8};
        int index = Arrays.binarySearch(arr, 3);
        System.out.println("Element found at index: " + index); // 2
    }
}
```

#### 3. Filling an Array (`Arrays.fill()`)
```java
import java.util.Arrays;
public class ArraysFillExample {
    public static void main(String[] args) {
        int[] arr = new int[5];
        Arrays.fill(arr, 7);
        System.out.println(Arrays.toString(arr)); // [7, 7, 7, 7, 7]
    }
}
```

#### 4. Comparing Arrays (`Arrays.equals()`)
```java
import java.util.Arrays;
public class ArraysEqualsExample {
    public static void main(String[] args) {
        int[] arr1 = {1, 2, 3};
        int[] arr2 = {1, 2, 3};
        System.out.println(Arrays.equals(arr1, arr2)); // true
    }
}
```

---

## 3. Final Arrays in Java
A `final` array means that the reference to the array cannot be changed, but its elements can still be modified.

### Example:
```java
public class FinalArrayExample {
    public static void main(String[] args) {
        final int[] arr = {1, 2, 3, 4, 5};
        
        // Modifying elements is allowed
        arr[0] = 10;
        System.out.println(Arrays.toString(arr)); // [10, 2, 3, 4, 5]
        
        // Trying to reassign will cause an error
        // arr = new int[]{6, 7, 8}; // Error: cannot assign a new array
    }
}
```

### Key Points:
- **You can modify the elements of a `final` array.**
- **You cannot reassign the reference of a `final` array.**

---

## Summary
| Feature            | Description |
|-------------------|-------------|
| **Jagged Arrays** | 2D arrays with variable column sizes |
| **Arrays Class**  | Provides utility methods like sorting, searching, filling, comparing, etc. |
| **Final Arrays**  | Prevents reassignment but allows modification of elements |

---

# Strings in Java

## What is a String in Java?
In Java, a `String` is a sequence of characters. It is one of the most commonly used data types and is part of `java.lang.String`.

Example:
```java
String str = "Hello, Java!";
System.out.println(str); // Output: Hello, Java!
```

## Immutability of Strings
Strings in Java are **immutable**, meaning once created, they cannot be changed.

Example:
```java
String s1 = "Hello";
s1.concat(" World"); // This does NOT modify s1
System.out.println(s1); // Output: Hello
```

If modification is needed, a new `String` object is created instead of modifying the original.

To modify strings efficiently, use `StringBuilder` or `StringBuffer`:
```java
StringBuilder sb = new StringBuilder("Hello");
sb.append(" World");
System.out.println(sb); // Output: Hello World
```

## String Class Methods
The `String` class provides various methods for string manipulation.

### 1. `length()` - Returns the length of the string.
```java
String str = "Java";
System.out.println(str.length()); // Output: 4
```

### 2. `charAt(index)` - Returns the character at a given index.
```java
String str = "Hello";
System.out.println(str.charAt(1)); // Output: e
```

### 3. `substring(start, end)` - Extracts a part of the string.
```java
String str = "Programming";
System.out.println(str.substring(3, 8)); // Output: gram
```

### 4. `toUpperCase()` and `toLowerCase()` - Converts to uppercase/lowercase.
```java
String str = "Java";
System.out.println(str.toUpperCase()); // Output: JAVA
System.out.println(str.toLowerCase()); // Output: java
```

### 5. `equals()` and `equalsIgnoreCase()` - Compares two strings.
```java
String s1 = "Hello";
String s2 = "hello";
System.out.println(s1.equals(s2)); // Output: false
System.out.println(s1.equalsIgnoreCase(s2)); // Output: true
```

### 6. `contains()` - Checks if a string contains another string.
```java
String str = "Java is fun";
System.out.println(str.contains("Java")); // Output: true
```

### 7. `startsWith()` and `endsWith()` - Checks how the string begins or ends.
```java
String str = "Java Programming";
System.out.println(str.startsWith("Java")); // Output: true
System.out.println(str.endsWith("ing")); // Output: true
```

### 8. `replace()` - Replaces occurrences of a character or substring.
```java
String str = "Java is powerful";
System.out.println(str.replace("Java", "Python")); // Output: Python is powerful
```

### 9. `split()` - Splits a string based on a delimiter.
```java
String str = "apple,banana,grape";
String[] fruits = str.split(",");
for (String fruit : fruits) {
    System.out.println(fruit);
}
```
**Output:**
```
apple
banana
grape
```

### 10. `trim()` - Removes leading and trailing spaces.
```java
String str = "  Hello World  ";
System.out.println(str.trim()); // Output: "Hello World"
```

## String Concatenation

1. Using `+` operator:
```java
String s1 = "Hello";
String s2 = " World";
String s3 = s1 + s2;
System.out.println(s3); // Output: Hello World
```

2. Using `concat()` method:
```java
String s1 = "Hello";
String s2 = " Java";
System.out.println(s1.concat(s2)); // Output: Hello Java
```

## String Comparison

### Using `==` (Checks reference, not value)
```java
String s1 = "Java";
String s2 = "Java";
System.out.println(s1 == s2); // Output: true (same reference in string pool)
```

### Using `equals()` (Checks actual content)
```java
String s1 = new String("Java");
String s2 = new String("Java");
System.out.println(s1.equals(s2)); // Output: true
```

## StringBuffer and StringBuilder
Since `String` is immutable, use `StringBuffer` or `StringBuilder` for efficient modifications.

### `StringBuffer` (Thread-safe, but slower)
```java
StringBuffer sb = new StringBuffer("Hello");
sb.append(" Java");
System.out.println(sb); // Output: Hello Java
```

### `StringBuilder` (Not thread-safe, but faster)
```java
StringBuilder sb = new StringBuilder("Hello");
sb.append(" Java");
System.out.println(sb); // Output: Hello Java
```

## Summary
- `String` is immutable.
- Use `StringBuilder` or `StringBuffer` for modifications.
- `String` class has many useful methods for manipulation.
- Always use `equals()` for string comparison instead of `==`.

---
# StringBuilder and StringBuffer in Java

## 1. Introduction
In Java, **String**, **StringBuilder**, and **StringBuffer** are used to handle and manipulate strings. However, they have differences in mutability and performance.

## 2. String (Immutable)
- A `String` in Java is **immutable**, meaning its value **cannot be changed** after creation.
- Every modification (concatenation, replacement, etc.) creates a new `String` object, increasing memory usage.

### Example:
```java
public class StringExample {
    public static void main(String[] args) {
        String s1 = "Hello";
        s1 = s1 + " World"; // Creates a new String object
        System.out.println(s1); // Output: Hello World
    }
}
```

---

## 3. StringBuilder (Mutable, Not Thread-Safe)
- `StringBuilder` allows string modifications without creating new objects, improving performance.
- It is **not thread-safe**, meaning it cannot be used in multi-threaded environments safely.

### Example:
```java
public class StringBuilderExample {
    public static void main(String[] args) {
        StringBuilder sb = new StringBuilder("Hello");
        sb.append(" World");
        System.out.println(sb); // Output: Hello World
    }
}
```

### Common Methods of `StringBuilder`
| Method | Description |
|--------|------------|
| `append(String s)` | Appends the specified string at the end |
| `insert(int offset, String s)` | Inserts a string at a specified index |
| `replace(int start, int end, String s)` | Replaces characters between start and end indices |
| `delete(int start, int end)` | Deletes characters from start to end index |
| `reverse()` | Reverses the string |
| `capacity()` | Returns the current capacity of the builder |

#### Example of Methods:
```java
public class StringBuilderMethods {
    public static void main(String[] args) {
        StringBuilder sb = new StringBuilder("Hello");
        sb.append(" Java");
        sb.insert(5, " Beautiful");
        sb.replace(6, 15, "Awesome");
        sb.delete(6, 13);
        sb.reverse();
        System.out.println(sb);
    }
}
```

---

## 4. StringBuffer (Mutable, Thread-Safe)
- `StringBuffer` works similarly to `StringBuilder` but is **thread-safe**, meaning it can be used in multi-threaded environments.
- It has the same methods as `StringBuilder` but uses synchronized methods for thread safety, making it slower in single-threaded applications.

### Example:
```java
public class StringBufferExample {
    public static void main(String[] args) {
        StringBuffer sb = new StringBuffer("Hello");
        sb.append(" World");
        System.out.println(sb); // Output: Hello World
    }
}
```

---

## 5. String vs StringBuilder vs StringBuffer

| Feature | `String` | `StringBuilder` | `StringBuffer` |
|---------|---------|---------------|--------------|
| Mutability | Immutable | Mutable | Mutable |
| Performance | Slow (creates new objects) | Fast (no new objects) | Slower than `StringBuilder` (thread-safe) |
| Thread-Safety | Yes (immutable) | No | Yes |
| Use Case | When immutability is needed | When frequent modifications are needed | When thread-safety is required |

---

## 6. When to Use What?
- **Use `String`** when values don’t change frequently.
- **Use `StringBuilder`** when you need fast and mutable string operations in a **single-threaded** environment.
- **Use `StringBuffer`** when working with strings in a **multi-threaded** environment where synchronization is needed.

### Example of Performance Difference
```java
public class PerformanceTest {
    public static void main(String[] args) {
        long startTime, endTime;

        // String performance test
        startTime = System.nanoTime();
        String str = "Java";
        for (int i = 0; i < 10000; i++) {
            str += i;
        }
        endTime = System.nanoTime();
        System.out.println("String Time: " + (endTime - startTime) + " ns");

        // StringBuilder performance test
        startTime = System.nanoTime();
        StringBuilder sb = new StringBuilder("Java");
        for (int i = 0; i < 10000; i++) {
            sb.append(i);
        }
        endTime = System.nanoTime();
        System.out.println("StringBuilder Time: " + (endTime - startTime) + " ns");
    }
}
```

**Output (Approximate time values):**
```
String Time: 150000000 ns
StringBuilder Time: 5000000 ns
```

---

## 7. Conclusion
- `String` is immutable and should be used when data does not change frequently.
- `StringBuilder` is fast and efficient for frequent modifications but not thread-safe.
- `StringBuffer` is thread-safe but slightly slower than `StringBuilder`.
---
# Object-Oriented Programming (OOP) in Java

Object-Oriented Programming (OOP) is a programming paradigm that revolves around objects and classes. Java follows OOP principles, making code modular, reusable, and easier to maintain.

## 1. Key OOP Concepts in Java
Java supports four main OOP concepts:

### 1.1 Encapsulation
Encapsulation is the concept of **hiding data** within a class and only exposing necessary parts through methods. This helps to prevent direct access to variables, ensuring data integrity.

#### Example:
```java
class BankAccount {
    private double balance; // Private variable

    public BankAccount(double initialBalance) {
        this.balance = initialBalance;
    }

    // Getter method
    public double getBalance() {
        return balance;
    }

    // Setter method
    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        }
    }
}

public class Main {
    public static void main(String[] args) {
        BankAccount account = new BankAccount(1000);
        account.deposit(500);
        System.out.println("Balance: " + account.getBalance());
    }
}
```

### 1.2 Inheritance
Inheritance allows a **child class to inherit properties and methods** from a parent class, promoting reusability and hierarchy.

#### Example:
```java
class Animal {
    void makeSound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Dog barks");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog myDog = new Dog();
        myDog.makeSound(); // Inherited method
        myDog.bark();
    }
}
```

### 1.3 Polymorphism
Polymorphism allows a method to **perform different behaviors based on the object calling it**. It can be achieved through **method overloading and method overriding**.

#### Method Overloading (Compile-time Polymorphism):
```java
class MathOperations {
    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }
}

public class Main {
    public static void main(String[] args) {
        MathOperations math = new MathOperations();
        System.out.println(math.add(5, 10));
        System.out.println(math.add(5, 10, 15));
    }
}
```

#### Method Overriding (Runtime Polymorphism):
```java
class Parent {
    void show() {
        System.out.println("Parent class");
    }
}

class Child extends Parent {
    @Override
    void show() {
        System.out.println("Child class");
    }
}

public class Main {
    public static void main(String[] args) {
        Parent obj = new Child(); // Upcasting
        obj.show(); // Calls overridden method
    }
}
```

### 1.4 Abstraction
Abstraction **hides the implementation details** and only shows the necessary functionality. It can be achieved through **abstract classes and interfaces**.

#### Using Abstract Class:
```java
abstract class Vehicle {
    abstract void start(); // Abstract method
}

class Car extends Vehicle {
    @Override
    void start() {
        System.out.println("Car starts with a key");
    }
}

public class Main {
    public static void main(String[] args) {
        Vehicle myCar = new Car();
        myCar.start();
    }
}
```

#### Using Interface:
```java
interface Animal {
    void makeSound(); // Abstract method
}

class Cat implements Animal {
    public void makeSound() {
        System.out.println("Meow");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal myCat = new Cat();
        myCat.makeSound();
    }
}
```

## 2. Key Differences Between OOP Concepts
| Concept       | Definition | Example |
|--------------|------------|------------|
| **Encapsulation** | Hiding data using private variables and providing access via methods | Private balance variable in `BankAccount` class |
| **Inheritance** | One class acquires properties of another | `Dog` class extends `Animal` class |
| **Polymorphism** | One method behaves differently in different classes | Overloading `add()` method, overriding `show()` method |
| **Abstraction** | Hiding implementation and showing only required details | Abstract class `Vehicle`, Interface `Animal` |

## 3. Summary
- **Encapsulation** protects data by using private variables.
- **Inheritance** promotes code reusability.
- **Polymorphism** allows method behavior to vary at runtime or compile-time.
- **Abstraction** hides implementation details, improving modularity.

These concepts together make Java a powerful **Object-Oriented Programming language**. 🚀
---
# Classes, Objects, Constructors, and Object Class in Java

## 1. Classes in Java
A **class** in Java is a blueprint for creating objects. It defines **fields (attributes)** and **methods (behaviors)**.

### Example:
```java
// Defining a class
class Car {
    String brand;
    int speed;
    
    void showDetails() {
        System.out.println("Brand: " + brand + ", Speed: " + speed);
    }
}
```

## 2. Objects in Java
An **object** is an instance of a class. It is created using the `new` keyword.

### Example:
```java
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car(); // Object creation
        myCar.brand = "Tesla";
        myCar.speed = 120;
        
        myCar.showDetails(); // Calling method
    }
}
```
### Output:
```
Brand: Tesla, Speed: 120
```

## 3. Constructors in Java
A **constructor** is a special method used to initialize objects. It has the same name as the class and does not have a return type.

### Types of Constructors:
1. **Default Constructor**: Automatically provided if no constructor is defined.
2. **Parameterized Constructor**: Accepts parameters to initialize attributes.
3. **Copy Constructor**: Creates an object by copying another object (not built-in but can be implemented manually).

### Example:
```java
class Car {
    String brand;
    int speed;
    
    // Parameterized Constructor
    Car(String brand, int speed) {
        this.brand = brand;
        this.speed = speed;
    }
    
    void showDetails() {
        System.out.println("Brand: " + brand + ", Speed: " + speed);
    }
}

public class Main {
    public static void main(String[] args) {
        Car car1 = new Car("BMW", 150);
        car1.showDetails();
    }
}
```
### Output:
```
Brand: BMW, Speed: 150
```

## 4. Object Class in Java
The `Object` class is the **parent class** of all Java classes. It provides useful methods like:
- `toString()` → Returns string representation.
- `equals(Object obj)` → Compares objects.
- `hashCode()` → Returns hash code of an object.
- `clone()` → Creates a copy of an object.

### Example:
```java
class Car {
    String brand;
    int speed;
    
    Car(String brand, int speed) {
        this.brand = brand;
        this.speed = speed;
    }
    
    @Override
    public String toString() {
        return "Brand: " + brand + ", Speed: " + speed;
    }
}

public class Main {
    public static void main(String[] args) {
        Car car1 = new Car("Audi", 180);
        System.out.println(car1.toString());
    }
}
```
### Output:
```
Brand: Audi, Speed: 180
```

## Summary:
| Concept       | Description |
|--------------|------------|
| **Class** | Blueprint for creating objects. |
| **Object** | Instance of a class. |
| **Constructor** | Initializes an object. |
| **Object Class** | Parent class of all Java classes with useful methods. |

---
# Abstraction in Java

## What is Abstraction?

Abstraction in Java is the process of hiding the implementation details and only showing the essential functionality to the user. It helps simplify a system by focusing on **what an object does** rather than **how it does it**.

### Real-Life Example of Abstraction

A **TV remote control** is a good example of abstraction. It provides buttons to control the TV, but the user doesn’t need to understand how the internal circuits work.

---

## Achieving Abstraction in Java

### 1. Abstract Classes
### 2. Interfaces

### Abstract Classes

- An **abstract class** is declared using the `abstract` keyword.
- It can have **both abstract and concrete methods**.
- Abstract methods **don’t have a body** and must be implemented by subclasses.
- Abstract classes **cannot be instantiated**.

#### Example of Abstract Class

```java
// Abstract class
abstract class RemoteControl {
    abstract void turnOn();
    abstract void turnOff();
}

// Concrete class
class TVRemote extends RemoteControl {
    @Override
    void turnOn() {
        System.out.println("TV is turned ON.");
    }

    @Override
    void turnOff() {
        System.out.println("TV is turned OFF.");
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        RemoteControl remote = new TVRemote();
        remote.turnOn();   // TV is turned ON.
        remote.turnOff();  // TV is turned OFF.
    }
}
```

---

### Interfaces in Java

- An **interface** is a blueprint for a class.
- It only contains **abstract methods (before Java 8)**.
- From **Java 8**, interfaces can have **default** and **static** methods.
- A class implements an interface using the `implements` keyword.
- Interfaces help in achieving **100% abstraction**.

#### Example of Interface

```java
// Interface
interface Shape {
    double calculateArea(); // Abstract method
}

// Class implementing the interface
class Circle implements Shape {
    private double radius;

    public Circle(double radius) {
        this.radius = radius;
    }

    public double calculateArea() {
        return Math.PI * radius * radius;
    }
}

class Rectangle implements Shape {
    private double length, width;

    public Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }

    public double calculateArea() {
        return length * width;
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        Shape c = new Circle(5);
        Shape r = new Rectangle(4, 6);

        System.out.println("Area of Circle: " + c.calculateArea());
        System.out.println("Area of Rectangle: " + r.calculateArea());
    }
}
```

#### Output:
```
Area of Circle: 78.54
Area of Rectangle: 24.0
```

---

## Differences: Abstract Class vs Interface

| Feature               | Abstract Class       | Interface               |
|----------------------|-------------------|----------------------|
| Methods             | Can have both abstract & concrete methods | Only abstract methods (Java 7 and earlier); default & static methods from Java 8 |
| Fields              | Can have instance variables | Only constants (public, static, final) |
| Inheritance         | Supports single inheritance | Supports multiple inheritance |
| Access Modifiers    | Can have private, protected, and public methods | Methods are public by default |
| Instantiation       | Cannot be instantiated | Cannot be instantiated |

---

## When to Use Abstraction?

- When you need to **hide implementation details** from the user.
- When multiple classes **share common behavior** but require different implementations.
- When designing a system that follows **Object-Oriented Programming (OOP)** principles.

### Example: Abstract Class vs Interface

#### Abstract Class Example

```java
abstract class Vehicle {
    abstract void drive();
}

class Car extends Vehicle {
    void drive() {
        System.out.println("Car is driving.");
    }
}
```

#### Interface Example

```java
interface Animal {
    void speak();
}

class Dog implements Animal {
    public void speak() {
        System.out.println("Dog barks.");
    }
}
```

---

## Advantages of Abstraction

✅ **Hides Implementation Details**: Simplifies complex code.

✅ **Increases Code Reusability**: Common functionalities can be reused.

✅ **Enhances Security**: Only exposes necessary functionality.

✅ **Improves Code Maintainability**: Easier to modify and extend.

✅ **Supports Loose Coupling**: Helps in designing loosely coupled systems.

---

## Disadvantages of Abstraction

❌ **Increased Complexity**: Too many abstract classes can make the code complex.

❌ **Overhead in Performance**: Extra layers of abstraction can slow down execution.

---

## Conclusion

- Abstraction in Java allows us to **hide implementation details** and **show only necessary features**.
- It can be achieved using **Abstract Classes** and **Interfaces**.
- **Abstract classes** allow partial abstraction, while **Interfaces** enable full abstraction.
- It enhances **security, maintainability, and reusability** in Java applications.

🚀 **Happy Coding!** 🎯
---
# Encapsulation in Java


Encapsulation in Java is a fundamental Object-Oriented Programming (OOP) principle that combines data and methods within a class. It allows implementation details to be hidden while exposing a public interface for interaction.

## Example: Simple Encapsulation in Java

```java
// Java program demonstrating Encapsulation
class Programmer {
    private String name;

    // Getter and Setter for name
    public String getName() { return name; }
    public void setName(String name) { this.name = name; }
}

public class Geeks {
    public static void main(String[] args) {
        Programmer p = new Programmer();
        p.setName("Geek");
        System.out.println("Name=> " + p.getName());
    }
}
```

### Output:
```
Name=> Geek
```

### Explanation:
- The class restricts direct access to its fields.
- The `getName()` and `setName()` methods (getters and setters) provide controlled access.
- This ensures data integrity and maintains encapsulation.

---

## Implementation of Encapsulation in Java
Encapsulation is implemented by declaring instance variables as **private**, restricting direct access. Public **getter** and **setter** methods are used to retrieve and modify these variables, allowing controlled access.

### Key Points:
- **Data hiding**: Prevents direct access to class variables.
- **Getter and Setter methods**: Used to access private data safely.
- **Security and flexibility**: Ensures better control over data.
- **Encapsulation vs Abstraction**: Encapsulation hides data, while abstraction hides implementation details.

## Example 1: Encapsulation with a `Person` Class

```java
// Java program to demonstrate Encapsulation.
class Person {
    private String name;
    private int age;

    public String getName() { return name; }
    public void setName(String name) { this.name = name; }

    public int getAge() { return age; }
    public void setAge(int age) { this.age = age; }
}

public class Geeks {
    public static void main(String[] args) {
        Person p = new Person();
        p.setName("John");
        p.setAge(30);

        System.out.println("Name: " + p.getName());
        System.out.println("Age: " + p.getAge());
    }
}
```

### Output:
```
Name: John
Age: 30
```

### Explanation:
- The `name` and `age` fields are **private**.
- Getters and setters control data access.
- Direct access to `name` and `age` is **not allowed**, ensuring data security.

---

## Example 2: Encapsulation with a `Rectangle` Class

```java
class Area {
    private int length;
    private int breadth;

    // Constructor to initialize values
    Area(int length, int breadth) {
        this.length = length;
        this.breadth = breadth;
    }

    // Method to calculate area
    public void getArea() {
        int area = length * breadth;
        System.out.println("Area: " + area);
    }
}

public class Geeks {
    public static void main(String[] args) {
        Area rect = new Area(2, 16);
        rect.getArea();
    }
}
```

### Output:
```
Area: 32
```

### Explanation:
- The variables `length` and `breadth` are private.
- The `getArea()` method calculates and prints the area.

---

## Example 3: Encapsulation with a `Student` Class

```java
// Java program demonstrating encapsulation
class Encapsulate {
    private String name;
    private int rollNo;
    private int age;

    // Getters
    public int getAge() { return age; }
    public String getName() { return name; }
    public int getRollNo() { return rollNo; }

    // Setters
    public void setAge(int newAge) { age = newAge; }
    public void setName(String newName) { name = newName; }
    public void setRollNo(int newRoll) { rollNo = newRoll; }
}

public class TestEncapsulation {
    public static void main(String[] args) {
        Encapsulate obj = new Encapsulate();
        obj.setName("Harsh");
        obj.setAge(19);
        obj.setRollNo(51);

        System.out.println("Name: " + obj.getName());
        System.out.println("Age: " + obj.getAge());
        System.out.println("Roll No: " + obj.getRollNo());
    }
}
```

### Output:
```
Name: Harsh
Age: 19
Roll No: 51
```

---

## Example 4: Encapsulation in a Banking System

```java
// Java program demonstrating encapsulation in a bank account system
class Account {
    private long accNo;
    private String name;
    private String email;
    private float balance;

    public long getAccNo() { return accNo; }
    public void setAccNo(long accNo) { this.accNo = accNo; }
    
    public String getName() { return name; }
    public void setName(String name) { this.name = name; }
    
    public String getEmail() { return email; }
    public void setEmail(String email) { this.email = email; }
    
    public float getBalance() { return balance; }
    public void setBalance(float balance) { this.balance = balance; }
}

public class BankApp {
    public static void main(String[] args) {
        Account acc = new Account();
        acc.setAccNo(90482098491L);
        acc.setName("ABC");
        acc.setEmail("abc@gmail.com");
        acc.setBalance(100000f);

        System.out.println("Account Number: " + acc.getAccNo());
        System.out.println("Name: " + acc.getName());
        System.out.println("Email: " + acc.getEmail());
        System.out.println("Balance: " + acc.getBalance());
    }
}
```

### Output:
```
Account Number: 90482098491
Name: ABC
Email: abc@gmail.com
Balance: 100000.0
```

---

## Advantages of Encapsulation
1. **Data Hiding**: Prevents unauthorized access to data.
2. **Data Integrity**: Ensures controlled modification through setters.
3. **Reusability**: Encapsulated code is easier to reuse.
4. **Improved Maintainability**: Changes in implementation do not affect external classes.
5. **Better Testing**: Encapsulated code is easier to test and debug.

## Disadvantages of Encapsulation
1. **Increased Code Complexity**: More lines of code due to getters and setters.
2. **Reduced Flexibility**: Direct access to variables is restricted.
3. **Performance Overhead**: Extra method calls for data access.

Encapsulation is a powerful concept in Java that ensures better data security, integrity, and code maintainability. 🚀

---
# Inheritance in Java


### What is Inheritance?
Inheritance is an important pillar of **Object-Oriented Programming (OOP)**. It is the mechanism in Java by which one class is allowed to **inherit** the properties (fields) and behavior (methods) of another class. 

In Java, **Inheritance** means creating new classes based on existing ones. The child class can reuse the methods and fields of the parent class and also define its own.

---

## Why Do We Need Java Inheritance?

1. **Code Reusability**: The code written in the superclass is common to all subclasses. Child classes can directly use the parent class code.
2. **Method Overriding**: Enables **runtime polymorphism**, where a child class can provide a specific implementation of a method.
3. **Abstraction**: Achieves abstraction by allowing higher-level classes to define common functionality without implementing all details.

---

## Important Terminologies in Java Inheritance

- **Class**: A blueprint for objects, defining fields and methods.
- **Super Class (Parent Class)**: The class whose members are inherited.
- **Sub Class (Child Class)**: The class that inherits from another class.
- **Reusability**: Inheritance enables reuse of fields and methods from the superclass.

---

## How to Use Inheritance in Java?
The `extends` keyword is used for inheritance in Java.

### Syntax:
```java
class DerivedClass extends BaseClass  
{  
   // methods and fields  
}  
```

### Example:
```java
// Java program to illustrate inheritance
class Bicycle {
    public int gear;
    public int speed;

    public Bicycle(int gear, int speed) {
        this.gear = gear;
        this.speed = speed;
    }

    public void applyBrake(int decrement) {
        speed -= decrement;
    }

    public void speedUp(int increment) {
        speed += increment;
    }

    public String toString() {
        return ("No of gears: " + gear + "\nSpeed: " + speed);
    }
}

// Derived class
class MountainBike extends Bicycle {
    public int seatHeight;

    public MountainBike(int gear, int speed, int startHeight) {
        super(gear, speed);
        seatHeight = startHeight;
    }

    public void setHeight(int newValue) {
        seatHeight = newValue;
    }

    @Override
    public String toString() {
        return (super.toString() + "\nSeat Height: " + seatHeight);
    }
}

// Driver class
public class Test {
    public static void main(String args[]) {
        MountainBike mb = new MountainBike(3, 100, 25);
        System.out.println(mb.toString());
    }
}
```

### Output:
```
No of gears: 3
Speed: 100
Seat Height: 25
```

---

## Types of Inheritance in Java
Java supports **five** types of inheritance:

### 1. **Single Inheritance**
A subclass inherits from one superclass.

```java
class One {
    public void printGeek() {
        System.out.println("Geeks");
    }
}

class Two extends One {
    public void printFor() {
        System.out.println("for");
    }
}

public class Main {
    public static void main(String[] args) {
        Two obj = new Two();
        obj.printGeek();
        obj.printFor();
    }
}
```

### Output:
```
Geeks
for
```

---

### 2. **Multilevel Inheritance**
A subclass inherits from another subclass.

```java
class One {
    public void printGeek() {
        System.out.println("Geeks");
    }
}

class Two extends One {
    public void printFor() {
        System.out.println("for");
    }
}

class Three extends Two {
    public void printGeekAgain() {
        System.out.println("Geeks");
    }
}

public class Main {
    public static void main(String[] args) {
        Three obj = new Three();
        obj.printGeek();
        obj.printFor();
        obj.printGeekAgain();
    }
}
```

### Output:
```
Geeks
for
Geeks
```

---

### 3. **Hierarchical Inheritance**
One superclass is inherited by multiple subclasses.

```java
class A {
    public void printA() {
        System.out.println("Class A");
    }
}

class B extends A {
    public void printB() {
        System.out.println("Class B");
    }
}

class C extends A {
    public void printC() {
        System.out.println("Class C");
    }
}

public class Test {
    public static void main(String[] args) {
        B objB = new B();
        objB.printA();
        objB.printB();

        C objC = new C();
        objC.printA();
        objC.printC();
    }
}
```

### Output:
```
Class A
Class B
Class A
Class C
```

---

### 4. **Multiple Inheritance (Through Interfaces)**
Java does not support multiple inheritances with classes but allows it using interfaces.

```java
interface One {
    void printGeek();
}

interface Two {
    void printFor();
}

class Child implements One, Two {
    public void printGeek() {
        System.out.println("Geeks");
    }
    public void printFor() {
        System.out.println("for");
    }
}

public class Main {
    public static void main(String[] args) {
        Child obj = new Child();
        obj.printGeek();
        obj.printFor();
    }
}
```

### Output:
```
Geeks
for
```

---

## Advantages of Inheritance
1. **Code Reusability**: Reduces code duplication.
2. **Abstraction**: Allows defining a common interface for related classes.
3. **Class Hierarchy**: Models real-world relationships.
4. **Polymorphism**: Enables method overriding for dynamic behavior.

## Disadvantages of Inheritance
1. **Complexity**: Can make the code harder to understand.
2. **Tight Coupling**: Changes in the superclass affect subclasses.

---

## Conclusion
- Java supports **single inheritance** through classes and **multiple inheritance** via interfaces.
- The `extends` keyword is used to inherit a class, and `super` invokes the superclass constructor.
- Private members are not inherited but can be accessed through getters and setters.

---
# Polymorphism in Java


## Introduction
The word **polymorphism** means "having many forms." In Java, polymorphism refers to the ability of a message or method to be displayed in more than one form. This is one of the key features of Object-Oriented Programming (OOP). It allows objects to behave differently based on their specific class type.

## Real-Life Example of Polymorphism
Consider a person who can have multiple roles simultaneously:
- A person can be a **father** to their child.
- A person can be a **husband** to their spouse.
- A person can be an **employee** at their workplace.

The same person exhibits different behaviors in different situations. This is an example of polymorphism.

## Example: A Person Having Different Roles

```java
// Base class Person
class Person {
    // Method to display the role of a person
    void role() {
        System.out.println("I am a person.");
    }
}

// Derived class Father that overrides the role method
class Father extends Person {
    @Override
    void role() {
        System.out.println("I am a father.");
    }
}

public class Main {
    public static void main(String[] args) {
        // Reference of type Person but object of type Father
        Person p = new Father();
        p.role();  // Calls the overridden method in Father class
    }
}
```

**Output:**
```
I am a father.
```

**Explanation:** The `Person` class has a method `role()` that prints a generic message. The `Father` class overrides `role()` to print a specific message. When we use a `Person` reference to hold a `Father` object, Java calls the overridden method in `Father`, demonstrating **runtime polymorphism**.

---

## Types of Polymorphism in Java
Java Polymorphism is mainly divided into two types:
1. **Compile-Time Polymorphism** (Static Polymorphism)
2. **Runtime Polymorphism** (Dynamic Polymorphism)

---

## 1. Compile-Time Polymorphism (Static Polymorphism)
Compile-Time Polymorphism in Java is also known as **method overloading**. This type of polymorphism is achieved by defining multiple methods with the same name but different parameters.

**Note:** Java does not support **operator overloading** like C++.

### Method Overloading
Method overloading occurs when multiple methods have the same name but different **number** or **type** of parameters.

### Example: Method Overloading by Changing the Number of Arguments

```java
// Class with overloaded methods
class Helper {
    // Method 1: With two integer parameters
    static int multiply(int a, int b) {
        return a * b;
    }

    // Method 2: With two double parameters
    static double multiply(double a, double b) {
        return a * b;
    }
}

// Main class
class Geeks {
    public static void main(String[] args) {
        System.out.println(Helper.multiply(2, 4));      // Calls int method
        System.out.println(Helper.multiply(5.5, 6.3));  // Calls double method
    }
}
```

**Output:**
```
8
34.65
```

### Subtypes of Compile-Time Polymorphism
- **Function Overloading:** Multiple methods with the same name but different parameters.
- **Operator Overloading:** (Not supported in Java, but available in C++).
- **Templates (Generics in Java):** Used for writing flexible, reusable code.

---

## 2. Runtime Polymorphism (Dynamic Method Dispatch)
Runtime Polymorphism in Java is also known as **Method Overriding**. In this type, the method call to an overridden method is resolved at runtime.

### Example: Method Overriding

```java
// Base class
class Parent {
    void print() {
        System.out.println("Parent class");
    }
}

// Subclass 1
class Subclass1 extends Parent {
    @Override
    void print() {
        System.out.println("Subclass1");
    }
}

// Subclass 2
class Subclass2 extends Parent {
    @Override
    void print() {
        System.out.println("Subclass2");
    }
}

// Main class
class Geeks {
    public static void main(String[] args) {
        Parent a;
        
        a = new Subclass1();
        a.print();  // Calls print() of Subclass1
        
        a = new Subclass2();
        a.print();  // Calls print() of Subclass2
    }
}
```

**Output:**
```
Subclass1
Subclass2
```

**Explanation:** When an object of a subclass is assigned to a reference of the superclass, the overridden method in the subclass gets called. This is **runtime polymorphism**.

### Subtype of Runtime Polymorphism
- **Virtual Functions:** Allow an object of a derived class to be treated as a base class object while still calling the overridden method.

---

## Advantages of Polymorphism
✅ Increases **code reusability** by allowing objects of different classes to be treated as a single class.
✅ Improves **readability and maintainability** by reducing redundant code.
✅ Supports **dynamic binding**, ensuring the correct method is called at runtime.
✅ Allows writing **generic code** that works with different object types.

## Disadvantages of Polymorphism
❌ Can make understanding object behavior difficult, especially in large codebases.
❌ May lead to **performance issues** due to additional computations at runtime.

---

## Summary
| Type of Polymorphism | Achieved By | Example |
|---------------------|-------------|---------|
| Compile-Time Polymorphism | Method Overloading | Multiple methods with the same name but different parameters |
| Runtime Polymorphism | Method Overriding | Subclass providing a different implementation of a method |

**Key Takeaway:** Polymorphism is a powerful concept that enhances flexibility, readability, and maintainability in Java programs.

---

## Conclusion
Polymorphism is an essential part of Java's Object-Oriented Programming paradigm. By understanding and implementing polymorphism, we can write efficient, scalable, and reusable code. 🚀
---
# Method Overloading and Method Overriding in Java

## What is Method Overloading?
Method overloading means defining multiple methods with the same name but different parameters in the same class.

### Key Points:
- It happens within the same class.
- Methods must have different numbers or types of parameters.
- It is an example of **compile-time polymorphism**.
- Return type alone cannot differentiate overloaded methods.

### Example of Method Overloading:
```java
class MathOperations {
    // Method with two int parameters
    int add(int a, int b) {
        return a + b;
    }
    
    // Overloaded method with three int parameters
    int add(int a, int b, int c) {
        return a + b + c;
    }
}

public class Main {
    public static void main(String[] args) {
        MathOperations obj = new MathOperations();
        System.out.println(obj.add(5, 10));    // Output: 15
        System.out.println(obj.add(5, 10, 15)); // Output: 30
    }
}
```

## What is Method Overriding?
Method overriding occurs when a subclass provides a specific implementation of a method that is already defined in its superclass.

### Key Points:
- It happens in **inheritance** (between superclass and subclass).
- The method name, return type, and parameters must be the same.
- The subclass method must have the **same access modifier** or a **less restrictive one**.
- It is an example of **runtime polymorphism**.

### Example of Method Overriding:
```java
class Animal {
    void makeSound() {
        System.out.println("Animals make sound");
    }
}

class Dog extends Animal {
    @Override
    void makeSound() {
        System.out.println("Dog barks");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal obj = new Dog();
        obj.makeSound(); // Output: Dog barks
    }
}
```

## Differences between Method Overloading and Method Overriding
| Feature             | Method Overloading        | Method Overriding          |
|--------------------|-------------------------|--------------------------|
| Definition        | Multiple methods with the same name but different parameters. | Subclass provides a new implementation for a method from the parent class. |
| Polymorphism Type | Compile-time polymorphism | Runtime polymorphism |
| Inheritance Required? | No | Yes |
| Return Type Matters? | No | Yes (should be the same or covariant) |
| Static Methods? | Yes, can be overloaded | No, static methods cannot be overridden |
| Access Modifier | No restriction | Must be same or less restrictive |

## Important Questions on Method Overloading and Overriding

### Q1: Can we overload static methods?
**Answer:** Yes, we can overload static methods. Example:
```java
class Test {
    static void display(int a) {
        System.out.println("Integer: " + a);
    }
    static void display(String a) {
        System.out.println("String: " + a);
    }
}
public class Main {
    public static void main(String[] args) {
        Test.display(10);
        Test.display("Hello");
    }
}
```
**Output:**
```
Integer: 10
String: Hello
```

### Q2: Can we overload methods that differ only by static keyword?
**Answer:** No, methods cannot be overloaded just by adding/removing `static`.

### Q3: Can we overload `main()` in Java?
**Answer:** Yes, but JVM only calls `main(String[] args)`. Example:
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Main with String[] args");
        main(10);
    }
    public static void main(int a) {
        System.out.println("Main with int: " + a);
    }
}
```
**Output:**
```
Main with String[] args
Main with int: 10
```

### Q4: Does Java support Operator Overloading?
**Answer:** No, Java does not support operator overloading except for `+` (used for string concatenation).

### Q5: Can we overload methods on return type?
**Answer:** No, return type alone cannot differentiate overloaded methods.
Example:
```java
class Test {
    int method() { return 10; }
    // char method() { return 'a'; }  // Error: Method already defined
}
```
However, it works when method parameters differ:
```java
class Test {
    int method(int a) { return a; }
    char method(int a, int b) { return 'a'; }
}
```

### Q6: What is the purpose of Method Overriding?
**Answer:** It allows subclasses to provide specific behavior for inherited methods. Example:
```java
class Employee {
    int getSalary() { return 30000; }
}
class Manager extends Employee {
    int getSalary() { return 50000; }
}
public class Main {
    public static void main(String[] args) {
        Employee e = new Manager();
        System.out.println(e.getSalary()); // Output: 50000
    }
}
```

## Conclusion
- **Method Overloading** provides flexibility by allowing multiple methods with the same name but different parameters.
- **Method Overriding** enables runtime polymorphism, allowing subclasses to provide their own implementations.

Both concepts are essential in Java to write clean, reusable, and maintainable code. 🚀
---
# Java Packages in Detail

## What is a Java Package?
A **package** in Java is a way to organize related classes and interfaces together. It helps to:
- Avoid name conflicts
- Improve code reusability
- Manage access control
- Make code easier to maintain

## Types of Java Packages
Java has two types of packages:
1. **Built-in Packages**: Predefined packages that come with Java (e.g., `java.util`, `java.io`).
2. **User-defined Packages**: Custom packages created by developers.

---

## 1. Built-in Packages
Java provides many built-in packages. Some commonly used ones are:

| Package Name  | Description |
|--------------|-------------|
| `java.lang`  | Core classes (Math, String, System, etc.) |
| `java.util`  | Utility classes (ArrayList, HashMap, Date, etc.) |
| `java.io`    | Input/Output (File handling, Streams, etc.) |
| `java.net`   | Networking (Socket programming, URL, etc.) |
| `java.sql`   | Database connectivity (JDBC API) |

### Example: Using `java.util` Package
```java
import java.util.ArrayList; // Importing ArrayList class

public class BuiltInPackageExample {
    public static void main(String[] args) {
        ArrayList<String> names = new ArrayList<>();
        names.add("Alice");
        names.add("Bob");
        System.out.println(names);
    }
}
```

---

## 2. User-defined Packages
You can create your own packages using the `package` keyword.

### Steps to Create a Package:
1. Declare the package name at the **beginning** of the Java file.
2. Save the file inside a folder with the **same name as the package**.
3. Compile and run the program correctly using the `javac` and `java` commands.

### Example: Creating and Using a Package
#### Step 1: Create a Package
Create a package named `mypackage` and save the file as `MyClass.java`.

```java
// File: MyClass.java
package mypackage; // Declaring package

public class MyClass {
    public void display() {
        System.out.println("Hello from MyClass in mypackage!");
    }
}
```

#### Step 2: Using the Package in Another File
Save this file as `Main.java` in the same directory as `mypackage`.

```java
// File: Main.java
import mypackage.MyClass; // Importing user-defined package

public class Main {
    public static void main(String[] args) {
        MyClass obj = new MyClass();
        obj.display();
    }
}
```

#### Step 3: Compile and Run
```sh
javac -d . MyClass.java Main.java  # Compile and store in correct package folder
java Main                          # Run the main program
```

**Output:**
```
Hello from MyClass in mypackage!
```

---

## Access Modifiers in Packages
| Access Modifier | Same Class | Same Package | Subclass (Different Package) | Different Package |
|----------------|-----------|-------------|------------------------|----------------|
| `public`       | ✅        | ✅          | ✅                      | ✅            |
| `protected`    | ✅        | ✅          | ✅                      | ❌            |
| Default (no keyword) | ✅  | ✅          | ❌                      | ❌            |
| `private`      | ✅        | ❌          | ❌                      | ❌            |

**Example:** Using `public` and `private` access modifiers in packages.
```java
package example;

public class PublicExample {
    public void showMessage() {
        System.out.println("This is a public method.");
    }
}

class PrivateExample {
    private void secretMessage() {
        System.out.println("This is a private method.");
    }
}
```

In another package, you **cannot** access `secretMessage()` because it is private.

---

## Importing Packages in Java
There are **three** ways to import a package:
1. **Import a specific class**
   ```java
   import java.util.ArrayList;
   ```
2. **Import an entire package**
   ```java
   import java.util.*; // Imports all classes from java.util
   ```
3. **Use fully qualified name (No import required)**
   ```java
   java.util.ArrayList<String> list = new java.util.ArrayList<>();
   ```

---

## Advantages of Using Packages
✅ **Code Reusability** – Easily use existing classes without rewriting them.
✅ **Name Conflict Resolution** – Prevents name conflicts by grouping related classes.
✅ **Access Control** – Defines visibility using access modifiers.
✅ **Encapsulation** – Hides implementation details.
✅ **Maintainability** – Organizes large projects into manageable units.

---

## Conclusion
Java packages are essential for organizing code efficiently. They help in structuring projects, avoiding naming conflicts, and managing access control. Built-in packages provide ready-to-use functionality, while user-defined packages allow better modularity and reusability in applications.

🚀 **Practice using packages to structure your Java projects efficiently!**
---
# Java Interfaces in Detail

## What is an Interface in Java?
An **interface** in Java is a blueprint for a class. It defines a set of abstract methods that the implementing class must provide. Interfaces help in achieving **multiple inheritance** and **abstraction** in Java.

### Syntax of an Interface
```java
// Declaring an Interface
interface Animal {
    void makeSound(); // Abstract method (No body)
}

// Implementing the Interface
class Dog implements Animal {
    public void makeSound() {
        System.out.println("Woof Woof!");
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        Dog d = new Dog();
        d.makeSound(); // Output: Woof Woof!
    }
}
```

## Interfaces and Inheritance
Interfaces support inheritance, allowing one interface to extend another.

### Example:
```java
interface ParentInterface {
    void method1();
}

// Child Interface extending Parent Interface
interface ChildInterface extends ParentInterface {
    void method2();
}

// Implementing the child interface
class ExampleClass implements ChildInterface {
    public void method1() {
        System.out.println("Method 1 implemented");
    }
    public void method2() {
        System.out.println("Method 2 implemented");
    }
}

public class Main {
    public static void main(String[] args) {
        ExampleClass obj = new ExampleClass();
        obj.method1(); // Output: Method 1 implemented
        obj.method2(); // Output: Method 2 implemented
    }
}
```

## Java Classes vs Interfaces
| Feature        | Class  | Interface |
|---------------|--------|------------|
| Methods      | Can have both abstract & concrete methods | Only abstract methods (until Java 8) |
| Multiple Inheritance | Not Supported | Supported |
| Variables    | Can have instance variables | Only public, static, and final variables |
| Constructors | Can have constructors | No constructors |

## Functional Interfaces in Java
A **Functional Interface** is an interface with only **one abstract method**. It is used in **lambda expressions**.

### Example:
```java
@FunctionalInterface
interface MyFunctionalInterface {
    void show();
}

public class Main {
    public static void main(String[] args) {
        MyFunctionalInterface obj = () -> System.out.println("Functional Interface Example");
        obj.show();
    }
}
```
**Output:** Functional Interface Example

## Nested Interfaces
An interface defined inside another interface or class is called a **nested interface**.

### Example:
```java
class OuterClass {
    interface InnerInterface {
        void show();
    }
}

class ImplementingClass implements OuterClass.InnerInterface {
    public void show() {
        System.out.println("Nested Interface Implemented");
    }
}

public class Main {
    public static void main(String[] args) {
        OuterClass.InnerInterface obj = new ImplementingClass();
        obj.show(); // Output: Nested Interface Implemented
    }
}
```

## Marker Interfaces
A **Marker Interface** is an interface with no methods. It is used to provide metadata to classes.

### Example:
```java
interface MarkerInterface {}

class ExampleClass implements MarkerInterface {
    public void display() {
        System.out.println("Marker Interface Example");
    }
}

public class Main {
    public static void main(String[] args) {
        ExampleClass obj = new ExampleClass();
        if (obj instanceof MarkerInterface) {
            obj.display(); // Output: Marker Interface Example
        }
    }
}
```

## Summary
- **Interfaces** define behavior that classes must implement.
- **Multiple interfaces** can be implemented in Java.
- **Functional Interfaces** allow lambda expressions.
- **Nested Interfaces** exist within a class or another interface.
- **Marker Interfaces** provide metadata without methods.

Interfaces play a crucial role in Java for achieving **abstraction, multiple inheritance, and better code structure**. 🚀
---
# Java Comparator Interface - Explained Simply

## What is the Comparator Interface?

The **Comparator** interface in Java is used to **customize the sorting order** of objects. It is found in the `java.util` package and provides a way to sort objects in **multiple ways**.

## Why Use Comparator?

1. **Custom Sorting:** Unlike `Comparable`, where sorting logic is inside the class, `Comparator` allows defining multiple sorting strategies.
2. **No Need to Modify Class:** You don't need to modify the original class to sort objects differently.
3. **More Flexible:** It allows sorting based on different attributes of the object.

## Comparator vs. Comparable

| Feature        | Comparable (`compareTo`) | Comparator (`compare`) |
|--------------|----------------|--------------|
| Where to Implement? | Inside the class of objects to be sorted | In a separate class or as an anonymous function |
| Method Used | `compareTo(Object o)` | `compare(Object o1, Object o2)` |
| Sorting Logic | Only one sorting logic | Multiple sorting logics |
| Modifies Class? | Yes, it modifies the original class | No, class remains unchanged |

## How to Use Comparator?

### Example: Sorting a List of Employees by Name and Salary

```java
import java.util.*;

// Employee class
class Employee {
    String name;
    int salary;

    Employee(String name, int salary) {
        this.name = name;
        this.salary = salary;
    }

    @Override
    public String toString() {
        return name + " - " + salary;
    }
}

// Comparator to sort by name
class NameComparator implements Comparator<Employee> {
    @Override
    public int compare(Employee e1, Employee e2) {
        return e1.name.compareTo(e2.name);
    }
}

// Comparator to sort by salary
class SalaryComparator implements Comparator<Employee> {
    @Override
    public int compare(Employee e1, Employee e2) {
        return Integer.compare(e1.salary, e2.salary);
    }
}

public class ComparatorExample {
    public static void main(String[] args) {
        List<Employee> employees = new ArrayList<>();
        employees.add(new Employee("Alice", 50000));
        employees.add(new Employee("Bob", 60000));
        employees.add(new Employee("Charlie", 40000));

        // Sorting by name
        Collections.sort(employees, new NameComparator());
        System.out.println("Sorted by Name: " + employees);

        // Sorting by salary
        Collections.sort(employees, new SalaryComparator());
        System.out.println("Sorted by Salary: " + employees);
    }
}
```

### Output:
```
Sorted by Name: [Alice - 50000, Bob - 60000, Charlie - 40000]
Sorted by Salary: [Charlie - 40000, Alice - 50000, Bob - 60000]
```

## Using Lambda Expression for Comparator (Java 8+)

Java 8 allows us to use **lambda expressions** to make sorting even simpler:

```java
Collections.sort(employees, (e1, e2) -> e1.name.compareTo(e2.name));
```
Or using `Comparator.comparing()` method:

```java
employees.sort(Comparator.comparing(e -> e.name));
```

### Sorting by Multiple Fields

We can also **chain comparators** to sort by multiple fields:

```java
employees.sort(Comparator.comparing(Employee::getName)
        .thenComparing(Employee::getSalary));
```

## Summary

- **Comparator** is useful for sorting objects in multiple ways.
- It provides more flexibility than `Comparable`.
- It is implemented separately, keeping the original class unchanged.
- Java 8 introduces lambda expressions to simplify sorting.
---
# Java Collections

## What is Java Collections Framework?
The **Java Collections Framework (JCF)** is a set of classes and interfaces that help store and manage groups of objects efficiently. It provides ready-made data structures like **List, Set, Queue, and Map** to handle collections of data.

### Key Features of Java Collections:
- **Reusable & Efficient**: Saves time by providing pre-built data structures.
- **Scalability**: Handles large amounts of data efficiently.
- **Dynamic Size**: Unlike arrays, collections can grow or shrink dynamically.

---

## **Hierarchy of Java Collections Framework**
### Collection Interface (Root Interface)
The **Collection Interface** is the parent of all collection classes in Java.

```
             Collection (Interface)
                  |
  ----------------------------------
  |               |                 |
 List           Queue              Set
(ArrayList)   (LinkedList)   (HashSet, TreeSet)
```

---

## **1. List Interface (Ordered Collection, Allows Duplicates)**
The **List** interface allows duplicate elements and maintains the insertion order.

### Implementations of List:
1. **ArrayList** (Fast for searching, slow for insert/delete)
2. **LinkedList** (Fast for insert/delete, slow for searching)
3. **Vector** (Thread-safe alternative to ArrayList)

### Example:
```java
import java.util.*;

public class ListExample {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        list.add("Apple");
        list.add("Banana");
        list.add("Apple"); // Duplicates Allowed
        System.out.println(list);
    }
}
```
**Output:** `[Apple, Banana, Apple]`

---

## **2. Set Interface (Unique Elements, No Duplicates)**
A **Set** doesn’t allow duplicate elements and doesn’t guarantee order.

### Implementations of Set:
1. **HashSet** (Fastest, No order maintained)
2. **LinkedHashSet** (Maintains insertion order)
3. **TreeSet** (Sorted order)

### Example:
```java
import java.util.*;

public class SetExample {
    public static void main(String[] args) {
        Set<String> set = new HashSet<>();
        set.add("Dog");
        set.add("Cat");
        set.add("Dog"); // Duplicate not added
        System.out.println(set);
    }
}
```
**Output:** `[Cat, Dog]` (Order may vary)

---

## **3. Queue Interface (FIFO - First In, First Out)**
A **Queue** follows the FIFO principle, where elements are added at the back and removed from the front.

### Implementations of Queue:
1. **LinkedList** (Can be used as a queue)
2. **PriorityQueue** (Elements are processed based on priority)

### Example:
```java
import java.util.*;

public class QueueExample {
    public static void main(String[] args) {
        Queue<Integer> queue = new LinkedList<>();
        queue.add(10);
        queue.add(20);
        queue.add(30);
        System.out.println(queue.poll()); // Removes 10
    }
}
```
**Output:** `10`

---

## **4. Map Interface (Key-Value Pairs)**
A **Map** stores elements in a key-value pair format, where keys are unique.

### Implementations of Map:
1. **HashMap** (Fastest, No order maintained)
2. **LinkedHashMap** (Maintains insertion order)
3. **TreeMap** (Sorted order by key)

### Example:
```java
import java.util.*;

public class MapExample {
    public static void main(String[] args) {
        Map<Integer, String> map = new HashMap<>();
        map.put(1, "One");
        map.put(2, "Two");
        map.put(1, "Updated One"); // Updates value of key 1
        System.out.println(map);
    }
}
```
**Output:** `{1=Updated One, 2=Two}` (Order may vary)

---

## **Comparing Collections: Which One to Use?**
| Collection Type | Allows Duplicates | Ordered? | Best Use Case |
|---------------|----------------|---------|--------------|
| **ArrayList** | Yes | Yes | Fast random access |
| **LinkedList** | Yes | Yes | Fast insertions/deletions |
| **HashSet** | No | No | Unique elements, fast lookup |
| **LinkedHashSet** | No | Yes | Unique elements, maintains order |
| **TreeSet** | No | Yes (Sorted) | Sorted unique elements |
| **HashMap** | Keys Unique | No | Key-Value storage |
| **TreeMap** | Keys Unique | Yes (Sorted) | Sorted key-value storage |

---

## **Advantages of Java Collections**
✔ Saves development time by providing pre-built data structures.
✔ Dynamic sizing (Unlike Arrays which have fixed sizes).
✔ Well-optimized for performance.
✔ Helps in writing cleaner, reusable, and maintainable code.

---

## **Conclusion**
The **Java Collections Framework** provides powerful tools for storing and managing data efficiently. Depending on the use case, choosing the right data structure can significantly improve performance and simplify the code.

### 🔥 Key Takeaways:
✔ **List** – Allows duplicates, maintains order.
✔ **Set** – No duplicates, no guaranteed order.
✔ **Queue** – Follows FIFO (First In First Out).
✔ **Map** – Stores key-value pairs.

Happy Coding! 🚀
---
# Java Collection Classes and Collection Interfaces

## 1. Introduction to Collections Framework
Java Collections Framework provides a set of interfaces and classes to store and manipulate groups of objects. It helps in handling dynamic data structures like **lists, sets, queues, and maps** efficiently.

## 2. Collection Interfaces in Java
Java provides multiple collection interfaces, which are the foundation of the **Collections Framework**.

### 2.1 `Collection` Interface
- Root interface of the Java Collection Framework.
- Provides methods like `add()`, `remove()`, `size()`, `iterator()`, etc.
- Extended by other interfaces like `List`, `Set`, and `Queue`.

```java
import java.util.*;

public class CollectionExample {
    public static void main(String[] args) {
        Collection<String> collection = new ArrayList<>();
        collection.add("Apple");
        collection.add("Banana");
        collection.add("Cherry");

        for (String fruit : collection) {
            System.out.println(fruit);
        }
    }
}
```

### 2.2 `List` Interface
- Ordered collection (also called a **sequence**).
- Allows **duplicate** elements.
- Implemented by `ArrayList`, `LinkedList`, `Vector`, `Stack`.

```java
import java.util.*;

public class ListExample {
    public static void main(String[] args) {
        List<Integer> list = new ArrayList<>();
        list.add(10);
        list.add(20);
        list.add(10); // Duplicate allowed

        System.out.println(list);
    }
}
```

### 2.3 `Set` Interface
- **No duplicates** allowed.
- Implemented by `HashSet`, `LinkedHashSet`, `TreeSet`.

```java
import java.util.*;

public class SetExample {
    public static void main(String[] args) {
        Set<String> set = new HashSet<>();
        set.add("Java");
        set.add("Python");
        set.add("Java"); // Duplicate not allowed

        System.out.println(set);
    }
}
```

### 2.4 `Queue` Interface
- **FIFO (First In First Out)** data structure.
- Implemented by `LinkedList`, `PriorityQueue`.

```java
import java.util.*;

public class QueueExample {
    public static void main(String[] args) {
        Queue<Integer> queue = new LinkedList<>();
        queue.add(1);
        queue.add(2);
        queue.add(3);

        System.out.println(queue.poll()); // Removes first element (FIFO)
    }
}
```

### 2.5 `Map` Interface
- Stores **key-value** pairs.
- **Keys are unique** but values can be duplicate.
- Implemented by `HashMap`, `LinkedHashMap`, `TreeMap`.

```java
import java.util.*;

public class MapExample {
    public static void main(String[] args) {
        Map<Integer, String> map = new HashMap<>();
        map.put(1, "One");
        map.put(2, "Two");
        map.put(1, "Uno"); // Overwrites key 1

        System.out.println(map);
    }
}
```

## 3. Collection Classes in Java
Java provides **concrete implementations** of the above interfaces in the `java.util` package.

### 3.1 `ArrayList`
- Implements `List`, uses **dynamic array**.
- Faster for **random access**, slower for **insertions/deletions**.

```java
List<String> list = new ArrayList<>();
```

### 3.2 `LinkedList`
- Implements `List`, **doubly linked list**.
- Faster **insertions/deletions**, slower **random access**.

```java
List<String> list = new LinkedList<>();
```

### 3.3 `HashSet`
- Implements `Set`, **unordered** collection.
- Uses **hashing** for fast operations.

```java
Set<String> set = new HashSet<>();
```

### 3.4 `TreeSet`
- Implements `Set`, **sorted order**.

```java
Set<String> set = new TreeSet<>();
```

### 3.5 `HashMap`
- Implements `Map`, **unordered** key-value store.
- **Fast retrieval** but no order guarantee.

```java
Map<Integer, String> map = new HashMap<>();
```

### 3.6 `TreeMap`
- Implements `Map`, **sorted key-value store**.

```java
Map<Integer, String> map = new TreeMap<>();
```

## 4. Differences Between Collection Classes
| Feature      | `ArrayList` | `LinkedList` | `HashSet` | `TreeSet` | `HashMap` | `TreeMap` |
|-------------|------------|------------|----------|---------|----------|---------|
| Order       | Yes        | Yes        | No       | Yes     | No       | Yes     |
| Duplicates  | Yes        | Yes        | No       | No      | Keys: No | Keys: No |
| Sorting     | No         | No         | No       | Yes     | No       | Yes     |
| Performance | Fast Access| Fast Insert/Delete | Fast | Slow (Sort) | Fast | Slow (Sort) |

## 5. Conclusion
- Use **ArrayList** for **fast access**, **LinkedList** for **fast insert/delete**.
- Use **HashSet** when **uniqueness** is needed, **TreeSet** for **sorted uniqueness**.
- Use **HashMap** for **fast key-value lookup**, **TreeMap** for **sorted key-value lookup**.

Java Collections Framework makes it easy to work with groups of objects efficiently! 🚀
---
# Java List, ArrayList, and Vector in Detail

## 1. List Interface in Java
The `List` interface is part of the Java Collections Framework and extends the `Collection` interface. It represents an ordered collection (also known as a sequence) and allows duplicate elements.

### **Characteristics of List**:
- Maintains insertion order.
- Allows duplicate elements.
- Provides positional access using indexes.
- Allows null values.

### **List Methods**:
- `add(E e)`: Adds an element.
- `get(int index)`: Retrieves an element.
- `remove(int index)`: Removes an element.
- `size()`: Returns the number of elements.
- `contains(Object o)`: Checks if an element exists.

### **Example Usage of List**:
```java
import java.util.*;

public class ListExample {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        list.add("Apple");
        list.add("Banana");
        list.add("Mango");
        list.add("Apple"); // Duplicates allowed

        System.out.println("List elements: " + list);
        System.out.println("Element at index 1: " + list.get(1));
        
        list.remove("Mango");
        System.out.println("After removing 'Mango': " + list);
    }
}
```

**Output:**
```
List elements: [Apple, Banana, Mango, Apple]
Element at index 1: Banana
After removing 'Mango': [Apple, Banana, Apple]
```

---
## 2. ArrayList in Java
`ArrayList` is a resizable array implementation of the `List` interface. It allows dynamic memory allocation.

### **Characteristics of ArrayList**:
- Uses a dynamic array for storage.
- Fast for retrieval (O(1) time complexity for `get()` method).
- Slower for insertions and deletions in the middle (O(n) time complexity).
- Not synchronized (not thread-safe).

### **Example Usage of ArrayList**:
```java
import java.util.ArrayList;

public class ArrayListExample {
    public static void main(String[] args) {
        ArrayList<Integer> numbers = new ArrayList<>();
        numbers.add(10);
        numbers.add(20);
        numbers.add(30);

        System.out.println("ArrayList: " + numbers);
        numbers.remove(1); // Removes element at index 1
        System.out.println("After removing element at index 1: " + numbers);
    }
}
```

**Output:**
```
ArrayList: [10, 20, 30]
After removing element at index 1: [10, 30]
```

---
## 3. Vector in Java
`Vector` is similar to `ArrayList`, but it is synchronized, making it thread-safe.

### **Characteristics of Vector**:
- Synchronized (thread-safe but slower than `ArrayList`).
- Uses a dynamic array for storage.
- Slower performance compared to `ArrayList` due to synchronization.

### **Example Usage of Vector**:
```java
import java.util.Vector;

public class VectorExample {
    public static void main(String[] args) {
        Vector<String> vector = new Vector<>();
        vector.add("Red");
        vector.add("Green");
        vector.add("Blue");

        System.out.println("Vector: " + vector);
        vector.remove("Green");
        System.out.println("After removing 'Green': " + vector);
    }
}
```

**Output:**
```
Vector: [Red, Green, Blue]
After removing 'Green': [Red, Blue]
```

---
## 4. Difference Between `ArrayList` and `Vector`
| Feature     | ArrayList | Vector |
|------------|----------|--------|
| Synchronization | Not synchronized (not thread-safe) | Synchronized (thread-safe) |
| Performance | Faster | Slower due to synchronization |
| Growth Rate | Increases by 50% | Doubles its size when needed |
| Iteration | Faster | Slower |

### **When to Use What?**
- Use `ArrayList` when **fast iteration and modification** are needed in a **single-threaded** environment.
- Use `Vector` when you need **thread-safe** operations in a **multi-threaded** environment.

---
## 5. Conclusion
- `List` is an interface that represents an **ordered collection**.
- `ArrayList` is a **resizable array**, suitable for **single-threaded applications**.
- `Vector` is **thread-safe** but has **lower performance** than `ArrayList`.
---
# Java Collections: Stack, LinkedList, Set, HashSet, TreeSet, and LinkedHashSet

## 1. Stack Class in Java
A **Stack** is a linear data structure that follows the **Last In, First Out (LIFO)** principle.

### **Key Methods of Stack:**
- `push(E item)`: Adds an item to the stack.
- `pop()`: Removes and returns the top item.
- `peek()`: Returns the top item without removing it.
- `isEmpty()`: Checks if the stack is empty.

### **Example of Stack:**
```java
import java.util.Stack;

public class StackExample {
    public static void main(String[] args) {
        Stack<Integer> stack = new Stack<>();
        stack.push(10);
        stack.push(20);
        stack.push(30);
        System.out.println("Stack: " + stack);
        System.out.println("Top Element: " + stack.peek());
        System.out.println("Popped Element: " + stack.pop());
        System.out.println("Stack after pop: " + stack);
    }
}
```
### **Output:**
```
Stack: [10, 20, 30]
Top Element: 30
Popped Element: 30
Stack after pop: [10, 20]
```

---

## 2. LinkedList Class in Java
A **LinkedList** is a doubly linked list implementation of the `List` and `Deque` interfaces.

### **Key Features:**
- Elements can be inserted/removed efficiently.
- Supports both `List` and `Queue` functionalities.

### **Example of LinkedList:**
```java
import java.util.LinkedList;

public class LinkedListExample {
    public static void main(String[] args) {
        LinkedList<String> list = new LinkedList<>();
        list.add("Apple");
        list.add("Banana");
        list.add("Cherry");
        System.out.println("LinkedList: " + list);
        list.remove("Banana");
        System.out.println("After removal: " + list);
    }
}
```
### **Output:**
```
LinkedList: [Apple, Banana, Cherry]
After removal: [Apple, Cherry]
```

---

## 3. Set Interface in Java
A **Set** is a collection that does **not allow duplicate elements**.

### **Types of Set Implementations:**
1. `HashSet`: Unordered, no duplicates.
2. `TreeSet`: Ordered in **ascending** order.
3. `LinkedHashSet`: Maintains insertion order.

---

## 4. HashSet in Java
A **HashSet** stores unique elements **without any specific order**.

### **Example of HashSet:**
```java
import java.util.HashSet;

public class HashSetExample {
    public static void main(String[] args) {
        HashSet<Integer> numbers = new HashSet<>();
        numbers.add(10);
        numbers.add(30);
        numbers.add(20);
        numbers.add(10); // Duplicate, won't be added
        System.out.println("HashSet: " + numbers);
    }
}
```
### **Output:**
```
HashSet: [20, 10, 30]
```

---

## 5. TreeSet in Java
A **TreeSet** maintains elements **in sorted order**.

### **Example of TreeSet:**
```java
import java.util.TreeSet;

public class TreeSetExample {
    public static void main(String[] args) {
        TreeSet<String> names = new TreeSet<>();
        names.add("Zebra");
        names.add("Apple");
        names.add("Mango");
        System.out.println("TreeSet (sorted order): " + names);
    }
}
```
### **Output:**
```
TreeSet (sorted order): [Apple, Mango, Zebra]
```

---

## 6. LinkedHashSet in Java
A **LinkedHashSet** maintains the insertion order.

### **Example of LinkedHashSet:**
```java
import java.util.LinkedHashSet;

public class LinkedHashSetExample {
    public static void main(String[] args) {
        LinkedHashSet<String> cities = new LinkedHashSet<>();
        cities.add("Delhi");
        cities.add("Mumbai");
        cities.add("Chennai");
        System.out.println("LinkedHashSet (Insertion Order): " + cities);
    }
}
```
### **Output:**
```
LinkedHashSet (Insertion Order): [Delhi, Mumbai, Chennai]
```

---

## **Summary:**
| Class          | Ordering       | Allows Duplicates? | Performance |
|---------------|---------------|-------------------|-------------|
| **Stack**     | LIFO          | Yes               | Fast for push/pop |
| **LinkedList**| Maintains order | Yes               | Good for frequent insertions/removals |
| **HashSet**   | No ordering   | No                | Fast lookup (O(1)) |
| **TreeSet**   | Sorted order  | No                | Slower (O(log n)) |
| **LinkedHashSet** | Insertion Order | No           | Maintains order (O(1)) |

This covers **Stack, LinkedList, Set, HashSet, TreeSet, and LinkedHashSet** in Java! 🚀 Let me know if you need more details! 😊
---
# Java Collections: Queue, Deque, PriorityQueue, Map, HashMap, LinkedHashMap, Hashtable, Java Dictionary Class, SortedSet Interface

## 1. Queue Interface in Java
Queue follows **FIFO (First-In-First-Out)** order. Elements are added at the rear and removed from the front.

### Example:
```java
import java.util.*;

public class QueueExample {
    public static void main(String[] args) {
        Queue<Integer> queue = new LinkedList<>();
        queue.add(10);
        queue.add(20);
        queue.add(30);

        System.out.println("Queue: " + queue);
        System.out.println("Removed: " + queue.poll()); // Removes first element
        System.out.println("Front Element: " + queue.peek()); // Peeks first element
    }
}
```

### Output:
```
Queue: [10, 20, 30]
Removed: 10
Front Element: 20
```
---
## 2. Deque Interface (Double-Ended Queue)
Deque allows insertion and deletion from both ends.

### Example:
```java
import java.util.*;

public class DequeExample {
    public static void main(String[] args) {
        Deque<String> deque = new LinkedList<>();
        deque.addFirst("Hello");
        deque.addLast("World");
        deque.addFirst("Java");

        System.out.println("Deque: " + deque);
        System.out.println("Removed First: " + deque.removeFirst());
        System.out.println("Removed Last: " + deque.removeLast());
    }
}
```

### Output:
```
Deque: [Java, Hello, World]
Removed First: Java
Removed Last: World
```
---
## 3. PriorityQueue (Min-Heap by default)
PriorityQueue maintains elements in **natural order** (ascending by default).

### Example:
```java
import java.util.*;

public class PriorityQueueExample {
    public static void main(String[] args) {
        PriorityQueue<Integer> pq = new PriorityQueue<>();
        pq.add(30);
        pq.add(10);
        pq.add(20);
        
        System.out.println("PriorityQueue: " + pq);
        System.out.println("Removed: " + pq.poll()); // Removes smallest element
    }
}
```

### Output:
```
PriorityQueue: [10, 30, 20]
Removed: 10
```
---
## 4. Map Interface (Key-Value Pairs)
Map stores **key-value pairs** where keys are unique.

### Example (HashMap):
```java
import java.util.*;

public class HashMapExample {
    public static void main(String[] args) {
        Map<Integer, String> map = new HashMap<>();
        map.put(1, "Java");
        map.put(2, "Python");
        map.put(3, "C++");

        System.out.println("Map: " + map);
        System.out.println("Value for key 2: " + map.get(2));
    }
}
```

### Output:
```
Map: {1=Java, 2=Python, 3=C++}
Value for key 2: Python
```
---
## 5. LinkedHashMap (Preserves Insertion Order)

### Example:
```java
import java.util.*;

public class LinkedHashMapExample {
    public static void main(String[] args) {
        LinkedHashMap<Integer, String> linkedHashMap = new LinkedHashMap<>();
        linkedHashMap.put(3, "C++");
        linkedHashMap.put(1, "Java");
        linkedHashMap.put(2, "Python");

        System.out.println("LinkedHashMap: " + linkedHashMap);
    }
}
```

### Output:
```
LinkedHashMap: {3=C++, 1=Java, 2=Python}
```
---
## 6. Hashtable (Thread-Safe, No Null Keys/Values)

### Example:
```java
import java.util.*;

public class HashtableExample {
    public static void main(String[] args) {
        Hashtable<Integer, String> hashtable = new Hashtable<>();
        hashtable.put(1, "Java");
        hashtable.put(2, "Python");

        System.out.println("Hashtable: " + hashtable);
    }
}
```

### Output:
```
Hashtable: {1=Java, 2=Python}
```
---
## 7. Java Dictionary Class (Legacy Collection)
Dictionary is a legacy abstract class that is replaced by `Map`.

### Example:
```java
import java.util.*;

public class DictionaryExample {
    public static void main(String[] args) {
        Dictionary<Integer, String> dictionary = new Hashtable<>();
        dictionary.put(1, "Java");
        dictionary.put(2, "Python");

        System.out.println("Dictionary: " + dictionary);
    }
}
```

### Output:
```
Dictionary: {1=Java, 2=Python}
```
---
## 8. SortedSet Interface (Maintains Sorted Order)
SortedSet stores elements in sorted order and does not allow duplicates.

### Example:
```java
import java.util.*;

public class SortedSetExample {
    public static void main(String[] args) {
        SortedSet<Integer> sortedSet = new TreeSet<>();
        sortedSet.add(50);
        sortedSet.add(10);
        sortedSet.add(30);

        System.out.println("SortedSet: " + sortedSet);
    }
}
```

### Output:
```
SortedSet: [10, 30, 50]
```
---
## Summary Table
| Collection Type | Description |
|---------------|-------------|
| **Queue** | FIFO-based collection |
| **Deque** | Double-ended queue |
| **PriorityQueue** | Min-Heap-based queue |
| **Map** | Stores key-value pairs (unordered) |
| **HashMap** | Unordered key-value pairs |
| **LinkedHashMap** | Ordered key-value pairs (insertion order) |
| **Hashtable** | Thread-safe version of HashMap |
| **Dictionary** | Legacy key-value storage class |
| **SortedSet** | Stores elements in sorted order |

---
# Comparator and Comparable in Java

## 1. Comparable Interface
The **Comparable** interface is used to define the **natural ordering** of objects. A class implementing `Comparable<T>` must override the `compareTo(T o)` method.

### Example of Comparable
```java
import java.util.*;

class Student implements Comparable<Student> {
    String name;
    int age;

    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    public int compareTo(Student s) {
        return this.age - s.age; // Sorting by age
    }

    public String toString() {
        return name + " - " + age;
    }
}

public class Main {
    public static void main(String[] args) {
        List<Student> students = new ArrayList<>();
        students.add(new Student("Alice", 25));
        students.add(new Student("Bob", 20));
        students.add(new Student("Charlie", 22));
        
        Collections.sort(students);
        System.out.println(students);
    }
}
```
### Output:
```
[Bob - 20, Charlie - 22, Alice - 25]
```

## 2. Comparator Interface
The **Comparator** interface provides a way to sort objects based on multiple conditions. It is useful when:
- We cannot modify the class (external sorting).
- We need multiple sorting logics.

### Example of Comparator
```java
import java.util.*;

class Student {
    String name;
    int age;

    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String toString() {
        return name + " - " + age;
    }
}

class AgeComparator implements Comparator<Student> {
    public int compare(Student s1, Student s2) {
        return s1.age - s2.age; // Sorting by age
    }
}

class NameComparator implements Comparator<Student> {
    public int compare(Student s1, Student s2) {
        return s1.name.compareTo(s2.name); // Sorting by name
    }
}

public class Main {
    public static void main(String[] args) {
        List<Student> students = new ArrayList<>();
        students.add(new Student("Alice", 25));
        students.add(new Student("Bob", 20));
        students.add(new Student("Charlie", 22));
        
        Collections.sort(students, new AgeComparator());
        System.out.println("Sorted by Age: " + students);
        
        Collections.sort(students, new NameComparator());
        System.out.println("Sorted by Name: " + students);
    }
}
```
### Output:
```
Sorted by Age: [Bob - 20, Charlie - 22, Alice - 25]
Sorted by Name: [Alice - 25, Bob - 20, Charlie - 22]
```

## 3. Comparator vs Comparable
| Feature | Comparable | Comparator |
|---------|-----------|------------|
| Package | `java.lang` | `java.util` |
| Method | `compareTo(Object o)` | `compare(Object o1, Object o2)` |
| Modification | Needs class modification | No modification required |
| Sorting Logic | Single sorting logic | Multiple sorting logics |
| Example | Sorting students by age | Sorting by age, name, etc. |

---

# Java Iterator
An **Iterator** is used to traverse a collection (List, Set, etc.) one element at a time.

## Example of Iterator
```java
import java.util.*;

public class IteratorExample {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        list.add("Apple");
        list.add("Banana");
        list.add("Cherry");

        Iterator<String> itr = list.iterator();
        while (itr.hasNext()) {
            System.out.println(itr.next());
        }
    }
}
```
### Output:
```
Apple
Banana
Cherry
```

## 4. Differences: Iterator vs ListIterator
| Feature | Iterator | ListIterator |
|---------|----------|-------------|
| Direction | Forward only | Both forward and backward |
| Methods | `hasNext()`, `next()`, `remove()` | `hasNext()`, `next()`, `hasPrevious()`, `previous()`, `add()`, `set()` |
| Applicable to | Any collection | Only `List` |

## Example of ListIterator
```java
import java.util.*;

public class ListIteratorExample {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        list.add("Apple");
        list.add("Banana");
        list.add("Cherry");

        ListIterator<String> listItr = list.listIterator();

        while (listItr.hasNext()) {
            System.out.println(listItr.next());
        }
    }
}
```

---

## Summary
- **Comparable** is used for natural sorting within a class (`compareTo()` method).
- **Comparator** is used for custom sorting (`compare()` method in separate classes).
- **Iterator** allows traversal through collections one element at a time.
- **ListIterator** allows bidirectional traversal.

This guide gives you a complete understanding of **Comparator, Comparable, and Iterators in Java**. 🚀 Happy Coding! 🎯
---
# Java Generics - A Complete Guide

## What are Java Generics?
Generics in Java allow us to create classes, interfaces, and methods that operate on parameters of different types while ensuring type safety at compile-time. It provides a way to write reusable and type-safe code.

### Example Without Generics:
```java
import java.util.*;

public class WithoutGenerics {
    public static void main(String[] args) {
        List list = new ArrayList();
        list.add("Hello");
        list.add(100); // No compile-time error
        
        String str = (String) list.get(0); // Type casting required
        System.out.println(str);
    }
}
```
#### Problems Without Generics:
- Requires **explicit type casting**, which may cause **runtime errors**.
- Code is **not type-safe**.

## How Generics Solve This Problem?
Generics allow defining a type parameter, ensuring **type safety** and eliminating explicit casting.

### Example With Generics:
```java
import java.util.*;

public class WithGenerics {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>(); // Type-safe list
        list.add("Hello");
        // list.add(100); // Compile-time error
        
        String str = list.get(0); // No need for type casting
        System.out.println(str);
    }
}
```
### Benefits of Generics:
✅ Type Safety
✅ Eliminates Type Casting
✅ Compile-time Type Checking
✅ Code Reusability

---

## Generic Classes
A generic class is defined with a **type parameter** inside `<>`.

### Example of a Generic Class:
```java
// Defining a generic class
class Box<T> {
    private T item;
    
    public void setItem(T item) {
        this.item = item;
    }
    
    public T getItem() {
        return item;
    }
}

public class GenericClassExample {
    public static void main(String[] args) {
        Box<String> stringBox = new Box<>();
        stringBox.setItem("Hello Generics");
        System.out.println(stringBox.getItem());
        
        Box<Integer> intBox = new Box<>();
        intBox.setItem(100);
        System.out.println(intBox.getItem());
    }
}
```
### Output:
```
Hello Generics
100
```

---

## Generic Methods
We can create methods that accept generic parameters.

### Example of a Generic Method:
```java
class GenericMethodExample {
    public static <T> void printArray(T[] array) {
        for (T element : array) {
            System.out.print(element + " ");
        }
        System.out.println();
    }
    
    public static void main(String[] args) {
        Integer[] intArray = {1, 2, 3, 4, 5};
        String[] strArray = {"A", "B", "C"};
        
        printArray(intArray);
        printArray(strArray);
    }
}
```
### Output:
```
1 2 3 4 5
A B C
```

---

## Bounded Type Parameters
We can restrict the types used in generics using **extends** keyword.

### Example:
```java
class BoundDemo<T extends Number> {
    private T num;
    
    public BoundDemo(T num) {
        this.num = num;
    }
    
    public double square() {
        return num.doubleValue() * num.doubleValue();
    }
}

public class BoundedTypeExample {
    public static void main(String[] args) {
        BoundDemo<Integer> intObj = new BoundDemo<>(5);
        System.out.println("Square: " + intObj.square());
        
        BoundDemo<Double> doubleObj = new BoundDemo<>(5.5);
        System.out.println("Square: " + doubleObj.square());
        
        // BoundDemo<String> strObj = new BoundDemo<>("Hello"); // Compile-time error
    }
}
```

---

## Wildcards in Generics
Wildcards (`?`) allow flexibility in generic type assignments.

### Example:
```java
import java.util.*;

class WildcardExample {
    public static void printList(List<?> list) {
        for (Object obj : list) {
            System.out.print(obj + " ");
        }
        System.out.println();
    }
    
    public static void main(String[] args) {
        List<Integer> intList = Arrays.asList(1, 2, 3);
        List<String> strList = Arrays.asList("A", "B", "C");
        
        printList(intList);
        printList(strList);
    }
}
```
### Output:
```
1 2 3
A B C
```

---

## Generic Interfaces
We can also create **generic interfaces**.

### Example:
```java
interface GenericInterface<T> {
    void display(T value);
}

class GenericClass<T> implements GenericInterface<T> {
    public void display(T value) {
        System.out.println("Value: " + value);
    }
}

public class GenericInterfaceExample {
    public static void main(String[] args) {
        GenericClass<Integer> obj = new GenericClass<>();
        obj.display(100);
        
        GenericClass<String> obj2 = new GenericClass<>();
        obj2.display("Hello");
    }
}
```
### Output:
```
Value: 100
Value: Hello
```

---

## Advantages of Java Generics
✅ **Code Reusability** – We can use the same class/method with different data types.
✅ **Type Safety** – Generics enforce type-checking at compile-time.
✅ **Elimination of Type Casting** – Reduces explicit type casting.
✅ **Better Performance** – No need for runtime type checks.

---

## Conclusion
Generics in Java provide type safety, code reusability, and cleaner syntax. It is widely used in Collections Framework, custom classes, and interfaces. Understanding generics helps in writing efficient and scalable Java programs.

---
# Java Exception Handling - Detailed Explanation

## What is Exception Handling?
Exception Handling in Java is a mechanism that allows a program to handle runtime errors (exceptions) gracefully without crashing. It ensures the normal flow of the application even when unexpected errors occur.

## What is an Exception?
An **exception** is an event that occurs during the execution of a program that disrupts the normal flow of instructions.

Example:
```java
int a = 10, b = 0;
int result = a / b; // This will throw an exception: ArithmeticException
```

## Why Use Exception Handling?
1. **Prevents Program Crash:** Handles errors without terminating the program abruptly.
2. **Improves Debugging:** Makes it easier to identify and fix errors.
3. **Enhances Code Readability:** Organizes error-handling code separately from business logic.
4. **Encourages Robust Applications:** Ensures the program can handle unexpected scenarios.

## Types of Exceptions
### 1. **Checked Exceptions**
- These exceptions are checked at compile-time.
- Must be handled using `try-catch` or `throws` keyword.
- Example: `IOException`, `SQLException`, `ClassNotFoundException`

Example:
```java
import java.io.*;
class CheckedExceptionExample {
    public static void main(String[] args) {
        try {
            FileReader file = new FileReader("test.txt");
        } catch (FileNotFoundException e) {
            System.out.println("File not found!");
        }
    }
}
```

### 2. **Unchecked Exceptions**
- These exceptions occur at runtime and are not checked at compile-time.
- Example: `ArithmeticException`, `NullPointerException`, `ArrayIndexOutOfBoundsException`, `IllegalArgumentException`

Example:
```java
class UncheckedExceptionExample {
    public static void main(String[] args) {
        int arr[] = {1, 2, 3};
        System.out.println(arr[5]); // ArrayIndexOutOfBoundsException
    }
}
```

### 3. **Errors**
- These are serious problems that cannot be handled.
- Example: `StackOverflowError`, `OutOfMemoryError`, `VirtualMachineError`

Example:
```java
class StackOverflowExample {
    public static void recursiveMethod() {
        recursiveMethod(); // Infinite recursion causes StackOverflowError
    }
    public static void main(String[] args) {
        recursiveMethod();
    }
}
```

## Exception Handling Keywords
### 1. `try`
Defines a block of code where an exception may occur.
```java
try {
    int a = 10 / 0;
} 
```

### 2. `catch`
Handles the exception thrown inside the `try` block.
```java
try {
    int a = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Cannot divide by zero");
}
```

### 3. `finally`
- Always executes regardless of whether an exception is thrown or not.
- Used to close resources.

```java
try {
    int a = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Cannot divide by zero");
} finally {
    System.out.println("This will always execute");
}
```

### 4. `throws`
- Declares exceptions that a method can throw.
- Used when we don't want to handle exceptions inside the method.

```java
void myMethod() throws IOException {
    throw new IOException("This is an IO exception");
}
```

### 5. `throw`
- Used to explicitly throw an exception.

```java
throw new ArithmeticException("Custom exception message");
```

## Multiple Catch Blocks
- A `try` block can have multiple `catch` blocks to handle different types of exceptions.
- The most specific exception should be caught first to avoid unreachable code errors.

```java
try {
    int a = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Arithmetic Exception");
} catch (Exception e) {
    System.out.println("General Exception");
}
```

## Nested Try-Catch
- We can nest `try-catch` blocks inside one another.
- Useful for handling exceptions at different levels of execution.

```java
class NestedTryCatchExample {
    public static void main(String[] args) {
        try {
            try {
                int a = 10 / 0;
            } catch (ArithmeticException e) {
                System.out.println("Inner catch: Arithmetic Exception");
            }
            int arr[] = new int[5];
            System.out.println(arr[10]); // Outer exception
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Outer catch: Array Index Out of Bounds");
        }
    }
}
```

## Custom Exceptions
- We can create user-defined exceptions by extending the `Exception` class.

```java
class MyException extends Exception {
    MyException(String message) {
        super(message);
    }
}

class Test {
    public static void main(String[] args) {
        try {
            throw new MyException("Custom Exception Occurred");
        } catch (MyException e) {
            System.out.println(e.getMessage());
        }
    }
}
```

## Best Practices for Exception Handling
1. **Catch Specific Exceptions**: Avoid using a generic `Exception` catch block.
2. **Use Finally Block for Cleanup**: Always close resources like database connections, files, etc.
3. **Log Exceptions**: Instead of suppressing exceptions, log them using `Logger`.
4. **Use Meaningful Exception Messages**: Provide useful messages when throwing exceptions.
5. **Do Not Ignore Exceptions**: Handle them properly to avoid undefined behavior.
6. **Avoid Using Too Many Nested Try-Catch Blocks**: Use well-structured error handling.

---
# `final`, `finally`, and `finalize` in Java - Detailed Explanation

Java provides three distinct concepts: `final`, `finally`, and `finalize`. Though they sound similar, they serve different purposes.

---
## **1. `final` Keyword**
The `final` keyword in Java is used to apply restrictions on classes, methods, and variables. Once assigned, its value cannot be changed.

### **Usage of `final` Keyword:**
- **Final Variable**: The value of a `final` variable cannot be changed once assigned.
- **Final Method**: A `final` method cannot be overridden by subclasses.
- **Final Class**: A `final` class cannot be extended.

### **1.1 Final Variable**
A `final` variable acts like a constant in Java. Once initialized, its value cannot be changed.

#### **Example:**
```java
class Test {
    final int speedLimit = 100; // Constant variable
    
    void changeSpeed() {
        // speedLimit = 120; // Compilation error, cannot change final variable
        System.out.println("Speed Limit: " + speedLimit);
    }
}
```

### **1.2 Final Method**
A `final` method cannot be overridden by subclasses, ensuring that the method's implementation remains unchanged.

#### **Example:**
```java
class Parent {
    final void show() {
        System.out.println("This is a final method");
    }
}

class Child extends Parent {
    // void show() { System.out.println("Trying to override"); } // Compilation error
}
```

### **1.3 Final Class**
A `final` class cannot be extended (inherited), which means no subclass can be created from it.

#### **Example:**
```java
final class Vehicle {
    void run() {
        System.out.println("Vehicle is running");
    }
}

// class Car extends Vehicle { } // Compilation error: Cannot inherit from final class
```

---
## **2. `finally` Block**
The `finally` block is used in exception handling. It ensures that some crucial code (like resource closing) executes whether an exception occurs or not.

### **Key Features of `finally`:**
- Always executes after `try` and `catch` blocks.
- Used to close resources such as database connections, files, etc.
- Executes even if `return`, `break`, or `continue` is used in `try` or `catch`.

### **Example of `finally` Block:**
```java
class FinallyExample {
    public static void main(String[] args) {
        try {
            int data = 10 / 0;
        } catch (ArithmeticException e) {
            System.out.println("Exception caught: " + e);
        } finally {
            System.out.println("Finally block executed");
        }
    }
}
```

### **Output:**
```
Exception caught: java.lang.ArithmeticException: / by zero
Finally block executed
```

---
## **3. `finalize()` Method**
The `finalize()` method is called by the Garbage Collector before an object is removed from memory. It is used to perform cleanup operations like closing resources before an object is destroyed.

### **Key Features of `finalize()`:**
- Defined in the `Object` class.
- Automatically called by the JVM before garbage collection.
- Can be overridden in a class to release resources.

### **Example of `finalize()` Method:**
```java
class FinalizeExample {
    protected void finalize() {
        System.out.println("Finalize method called");
    }
    
    public static void main(String[] args) {
        FinalizeExample obj = new FinalizeExample();
        obj = null; // Making object eligible for garbage collection
        System.gc(); // Requesting JVM for garbage collection
    }
}
```

### **Output:**
```
Finalize method called
```
(Note: The exact execution time of `finalize()` is not guaranteed.)

---
## **Difference Between `final`, `finally`, and `finalize`**
| Feature     | `final` | `finally` | `finalize()` |
|------------|--------|----------|-------------|
| Usage | Used for constants, methods, and classes | Used in exception handling | Used for garbage collection cleanup |
| Function | Prevents modification (immutable) | Ensures execution of important code | Called before an object is garbage collected |
| Where Used | Variables, Methods, Classes | `try-catch-finally` blocks | Method inside a class |
| Can Be Overridden? | No (for methods) | Not applicable | Yes |
| Execution Time | During compilation | During runtime exception handling | Before object destruction (by JVM) |

---
## **Summary**
- `final` is a keyword used to declare constants, prevent method overriding, and prevent inheritance.
- `finally` is a block used in exception handling to execute important code regardless of an exception.
- `finalize()` is a method that is invoked before an object is garbage collected.

---
# Chained Exception & Exception Handling with Method Overriding in Java - Detailed Explanation

Exception handling in Java provides advanced features like **Chained Exceptions** and **Exception Handling with Method Overriding**, which help in better debugging and structured error handling.

---
## **1. Chained Exceptions in Java**

### **What is Chained Exception?**
- A **Chained Exception** is used when one exception causes another exception.
- It helps preserve the original cause of an exception.
- It is useful for debugging when the actual cause of an exception is different from where it was caught.

### **How to Implement Chained Exceptions?**
Java provides constructors in the `Throwable` class to support exception chaining:

1. `Throwable(String message, Throwable cause)`
2. `Throwable(Throwable cause)`

### **Example of Chained Exception**
```java
class ChainedExceptionExample {
    public static void main(String[] args) {
        try {
            method1();
        } catch (Exception e) {
            System.out.println("Caught Exception: " + e);
            System.out.println("Original Cause: " + e.getCause());
        }
    }
    
    static void method1() throws Exception {
        try {
            int a = 5 / 0; // This will cause ArithmeticException
        } catch (ArithmeticException e) {
            throw new Exception("Custom Exception: Division by zero", e);
        }
    }
}
```

### **Output:**
```
Caught Exception: java.lang.Exception: Custom Exception: Division by zero
Original Cause: java.lang.ArithmeticException: / by zero
```

### **Why Use Chained Exceptions?**
- Helps in tracking the root cause of exceptions.
- Provides better debugging information.
- Ensures clarity when exceptions are thrown from different layers of an application (e.g., Database → Service → Controller).

---
## **2. Exception Handling with Method Overriding**

### **What is Exception Handling with Method Overriding?**
- When a method is overridden in a subclass, it can also change the exception-handling behavior.
- The overriding method must follow certain rules regarding checked exceptions.

### **Rules for Exception Handling with Method Overriding**
1. **If the parent method does not declare an exception:**
   - The overridden method **cannot** declare a checked exception.

2. **If the parent method declares an exception:**
   - The overridden method **can** declare the same exception or its subclass.
   - The overridden method **cannot** declare a broader (more general) exception.

3. **Unchecked exceptions:**
   - Can be declared in the overridden method without restriction.

### **Example 1: Overriding Method without Exception**
```java
class Parent {
    void show() {
        System.out.println("Parent method");
    }
}
class Child extends Parent {
    void show() throws ArithmeticException { // Allowed, unchecked exception
        System.out.println("Child method");
    }
}
class Test {
    public static void main(String[] args) {
        Parent p = new Child();
        p.show();
    }
}
```

### **Example 2: Overriding Method with Checked Exception**
```java
import java.io.*;
class Parent {
    void show() throws IOException {
        System.out.println("Parent method");
    }
}
class Child extends Parent {
    void show() throws FileNotFoundException { // Allowed, subclass of IOException
        System.out.println("Child method");
    }
}
```

### **Example 3: Overriding Method with Broader Exception (Not Allowed)**
```java
import java.io.*;
class Parent {
    void show() throws IOException {
        System.out.println("Parent method");
    }
}
class Child extends Parent {
    // void show() throws Exception { // Compilation error: broader exception
    //     System.out.println("Child method");
    // }
}
```

### **Summary of Method Overriding with Exception Handling**
| Parent Method Exception | Allowed in Child Method |
|------------------------|------------------------|
| No exception | Unchecked exception allowed, but not checked exceptions |
| `IOException` | `IOException` or subclass (e.g., `FileNotFoundException`) |
| `Exception` | `Exception` or subclass (e.g., `IOException`) |
| `RuntimeException` | Any unchecked exception (e.g., `ArithmeticException`) |

---
## **Key Differences Between Chained Exceptions and Exception Handling with Overriding**
| Feature | Chained Exception | Exception Handling in Overriding |
|---------|------------------|---------------------------------|
| Purpose | Preserve root cause of exception | Control exception propagation in inheritance |
| Usage | One exception causes another | Subclass modifies exception behavior of parent class |
| Methods Used | `getCause()` | Overriding rules apply |
| Exception Type | Any exception | Checked exceptions follow strict rules |

---
## **Conclusion**
- **Chained Exceptions** help track the original cause of an exception.
- **Exception Handling with Method Overriding** follows strict rules to ensure subclass exceptions remain compatible with the parent class.
- Proper handling of these concepts ensures **better debugging, maintainability, and clarity** in Java programs.
---
# File Handling in Java - Detailed Explanation

File handling in Java allows us to create, read, write, and manipulate files efficiently. Java provides the `java.io` and `java.nio` packages to perform file operations.

---
## **1. File Handling Classes in Java**
Java provides several classes for file handling:

| Class | Description |
|--------|-------------|
| `File` | Represents a file or directory |
| `FileReader` | Reads character data from a file |
| `FileWriter` | Writes character data to a file |
| `BufferedReader` | Reads text from a character input stream efficiently |
| `BufferedWriter` | Writes text to an output stream efficiently |
| `FileInputStream` | Reads binary data from a file |
| `FileOutputStream` | Writes binary data to a file |
| `RandomAccessFile` | Reads and writes data at any position in a file |
| `Files` (NIO) | Provides static methods for file operations |

---
## **2. Creating a File in Java**
We use the `File` class to create a new file.

### **Example:**
```java
import java.io.File;
import java.io.IOException;
class CreateFileExample {
    public static void main(String[] args) {
        try {
            File file = new File("example.txt");
            if (file.createNewFile()) {
                System.out.println("File created: " + file.getName());
            } else {
                System.out.println("File already exists.");
            }
        } catch (IOException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        }
    }
}
```

---
## **3. Writing to a File**
We use the `FileWriter` or `BufferedWriter` classes to write data to a file.

### **Example:**
```java
import java.io.FileWriter;
import java.io.IOException;
class WriteFileExample {
    public static void main(String[] args) {
        try {
            FileWriter writer = new FileWriter("example.txt");
            writer.write("Hello, this is a test file.");
            writer.close();
            System.out.println("Successfully written to the file.");
        } catch (IOException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        }
    }
}
```

---
## **4. Reading from a File**
We use `FileReader` or `BufferedReader` to read data from a file.

### **Example:**
```java
import java.io.FileReader;
import java.io.BufferedReader;
import java.io.IOException;
class ReadFileExample {
    public static void main(String[] args) {
        try {
            BufferedReader reader = new BufferedReader(new FileReader("example.txt"));
            String line;
            while ((line = reader.readLine()) != null) {
                System.out.println(line);
            }
            reader.close();
        } catch (IOException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        }
    }
}
```

---
## **5. Deleting a File**
We use the `delete()` method of the `File` class to delete a file.

### **Example:**
```java
import java.io.File;
class DeleteFileExample {
    public static void main(String[] args) {
        File file = new File("example.txt");
        if (file.delete()) {
            System.out.println("Deleted the file: " + file.getName());
        } else {
            System.out.println("Failed to delete the file.");
        }
    }
}
```

---
## **6. File Handling with `Files` Class (NIO)**
The `Files` class provides advanced methods for file operations.

### **Example:**
```java
import java.nio.file.*;
import java.io.IOException;
class NIOFileExample {
    public static void main(String[] args) {
        Path path = Paths.get("example.txt");
        try {
            Files.write(path, "Hello, NIO!".getBytes());
            String content = new String(Files.readAllBytes(path));
            System.out.println("File Content: " + content);
        } catch (IOException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        }
    }
}
```

---
## **7. Summary of File Handling in Java**
- `File` class is used to create, delete, and get information about a file.
- `FileWriter` and `BufferedWriter` are used for writing text data.
- `FileReader` and `BufferedReader` are used for reading text data.
- `FileInputStream` and `FileOutputStream` are used for binary data.
- `Files` class (NIO) provides modern file operations.


| Class | Description |
|--------|-------------|
| `File` | Represents a file or directory |
| `FileReader` | Reads character data from a file |
| `FileWriter` | Writes character data to a file |
| `BufferedReader` | Reads text from a character input stream efficiently |
| `BufferedWriter` | Writes text to an output stream efficiently |
| `FileInputStream` | Reads binary data from a file |
| `FileOutputStream` | Writes binary data to a file |
| `RandomAccessFile` | Reads and writes data at any position in a file |
| `FileDescriptor` | Represents a handle to an open file |
| `Files` (NIO) | Provides static methods for file operations |

---
## **2. FileReader in Java**
The `FileReader` class is used to read character data from a file.

### **Example:**
```java
import java.io.FileReader;
import java.io.IOException;
class FileReaderExample {
    public static void main(String[] args) {
        try (FileReader reader = new FileReader("example.txt")) {
            int ch;
            while ((ch = reader.read()) != -1) {
                System.out.print((char) ch);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

---
## **3. FileWriter in Java**
The `FileWriter` class is used to write character data to a file.

### **Example:**
```java
import java.io.FileWriter;
import java.io.IOException;
class FileWriterExample {
    public static void main(String[] args) {
        try (FileWriter writer = new FileWriter("example.txt")) {
            writer.write("Hello, FileWriter!");
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

---
## **4. FilePermission in Java**
The `FilePermission` class represents access rights to a file or directory.

### **Example:**
```java
import java.io.FilePermission;
import java.security.PermissionCollection;
class FilePermissionExample {
    public static void main(String[] args) {
        FilePermission permission = new FilePermission("example.txt", "read, write");
        System.out.println("Permission: " + permission.getActions());
    }
}
```

---
## **5. FileDescriptor in Java**
The `FileDescriptor` class represents a handle to an open file.

### **Example:**
```java
import java.io.*;
class FileDescriptorExample {
    public static void main(String[] args) {
        try {
            FileOutputStream fos = new FileOutputStream("example.txt");
            FileDescriptor fd = fos.getFD();
            fos.write("FileDescriptor example".getBytes());
            fos.flush();
            fd.sync();
            fos.close();
            System.out.println("FileDescriptor synced and closed.");
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

---
## **6. Summary of File Handling in Java**
- `FileReader` is used for reading character data.
- `FileWriter` is used for writing character data.
- `FilePermission` controls access rights to files.
- `FileDescriptor` represents a low-level handle to an open file.
---
# Multithreading in Java - Detailed Explanation

Multithreading is a process of executing multiple threads simultaneously to perform concurrent tasks. In Java, multithreading is implemented using the `Thread` class and `Runnable` interface.

---
## **1. What is Multithreading?**
Multithreading allows a program to perform multiple tasks concurrently, utilizing CPU resources efficiently. Each task runs as an independent thread within the same process.

### **Advantages of Multithreading:**
- Better CPU utilization
- Faster execution of independent tasks
- Improved performance in multi-core systems
- Helps in responsive GUI applications

---
## **2. Java Threads**
A thread is the smallest unit of a process that can execute independently. Java provides built-in support for multithreading using the `Thread` class and `Runnable` interface.

### **Thread Lifecycle:**
A thread in Java goes through several states:

| State | Description |
|--------|-------------|
| **New** | Thread object is created but not started |
| **Runnable** | Thread is ready to run but waiting for CPU |
| **Blocked** | Thread is waiting for a resource |
| **Waiting** | Thread is waiting indefinitely for another thread’s signal |
| **Timed Waiting** | Thread is waiting for a specified time |
| **Terminated** | Thread execution is completed |

---
## **3. Creating Threads in Java**
Java provides two ways to create threads:
1. Extending the `Thread` class
2. Implementing the `Runnable` interface

### **Using `Thread` Class**
```java
class MyThread extends Thread {
    public void run() {
        System.out.println("Thread is running...");
    }
    public static void main(String[] args) {
        MyThread t1 = new MyThread();
        t1.start(); // Starts the thread
    }
}
```

### **Using `Runnable` Interface**
```java
class MyRunnable implements Runnable {
    public void run() {
        System.out.println("Runnable thread is running...");
    }
    public static void main(String[] args) {
        Thread t1 = new Thread(new MyRunnable());
        t1.start(); // Starts the thread
    }
}
```

---
## **4. Thread Methods in Java**
Java provides several useful methods for managing threads:

| Method | Description |
|--------|-------------|
| `start()` | Starts the execution of a thread |
| `run()` | Defines the thread’s task |
| `sleep(ms)` | Puts the thread to sleep for a specified time |
| `join()` | Waits for a thread to complete execution |
| `isAlive()` | Checks if a thread is still running |
| `setName()` | Assigns a name to the thread |
| `getName()` | Gets the thread’s name |
| `setPriority()` | Sets thread priority (1 to 10) |
| `getPriority()` | Gets the priority of the thread |

---
## **5. Thread Synchronization**
When multiple threads access shared resources, data inconsistency may occur. Java provides synchronization mechanisms to avoid this issue.

### **Example of Synchronization:**
```java
class SharedResource {
    synchronized void printNumbers(int n) {
        for (int i = 1; i <= 5; i++) {
            System.out.println(n * i);
            try { Thread.sleep(500); } catch (Exception e) {}
        }
    }
}
class MyThread1 extends Thread {
    SharedResource obj;
    MyThread1(SharedResource obj) { this.obj = obj; }
    public void run() { obj.printNumbers(5); }
}
class MyThread2 extends Thread {
    SharedResource obj;
    MyThread2(SharedResource obj) { this.obj = obj; }
    public void run() { obj.printNumbers(10); }
}
class SyncExample {
    public static void main(String args[]) {
        SharedResource obj = new SharedResource();
        MyThread1 t1 = new MyThread1(obj);
        MyThread2 t2 = new MyThread2(obj);
        t1.start();
        t2.start();
    }
}
```

---
## **6. Thread Communication**
Java allows communication between threads using methods like `wait()`, `notify()`, and `notifyAll()`.

### **Example of Thread Communication:**
```java
class SharedData {
    int number;
    boolean isProduced = false;
    synchronized void produce(int num) {
        while (isProduced) {
            try { wait(); } catch (Exception e) {}
        }
        this.number = num;
        isProduced = true;
        System.out.println("Produced: " + num);
        notify();
    }
    synchronized void consume() {
        while (!isProduced) {
            try { wait(); } catch (Exception e) {}
        }
        System.out.println("Consumed: " + number);
        isProduced = false;
        notify();
    }
}
class Producer extends Thread {
    SharedData data;
    Producer(SharedData data) { this.data = data; }
    public void run() {
        for (int i = 1; i <= 5; i++) {
            data.produce(i);
            try { Thread.sleep(1000); } catch (Exception e) {}
        }
    }
}
class Consumer extends Thread {
    SharedData data;
    Consumer(SharedData data) { this.data = data; }
    public void run() {
        for (int i = 1; i <= 5; i++) {
            data.consume();
            try { Thread.sleep(1000); } catch (Exception e) {}
        }
    }
}
class ThreadCommExample {
    public static void main(String args[]) {
        SharedData data = new SharedData();
        Producer p = new Producer(data);
        Consumer c = new Consumer(data);
        p.start();
        c.start();
    }
}
```

---
## **7. Summary of Multithreading in Java**
- Java supports multithreading using the `Thread` class and `Runnable` interface.
- Thread states include New, Runnable, Blocked, Waiting, Timed Waiting, and Terminated.
- Thread methods like `start()`, `join()`, `sleep()`, and `synchronized` are crucial for controlling threads.
- Synchronization ensures data consistency in multithreaded programs.
- Thread communication allows proper coordination between producer and consumer threads.

---
## **1. Main Thread in Java**
In Java, the main thread is the first thread that starts when a program executes. It is responsible for invoking the `main()` method.

### **Example: Identifying the Main Thread**
```java
class MainThreadExample {
    public static void main(String[] args) {
        Thread t = Thread.currentThread();
        System.out.println("Current Thread: " + t.getName());
    }
}
```
### **Output:**
```
Current Thread: main
```
---
## **2. Java Thread Priority**
Java threads have priorities ranging from 1 to 10, where:
- `MIN_PRIORITY` = 1
- `NORM_PRIORITY` = 5 (default)
- `MAX_PRIORITY` = 10

### **Example: Setting and Getting Thread Priority**
```java
class PriorityExample extends Thread {
    public void run() {
        System.out.println(Thread.currentThread().getName() + " Priority: " + Thread.currentThread().getPriority());
    }
    public static void main(String args[]) {
        PriorityExample t1 = new PriorityExample();
        PriorityExample t2 = new PriorityExample();
        
        t1.setPriority(Thread.MIN_PRIORITY);
        t2.setPriority(Thread.MAX_PRIORITY);
        
        t1.start();
        t2.start();
    }
}
```
---
## **3. Naming a Thread and Fetching Thread Name**
We can assign custom names to threads and fetch their names using `setName()` and `getName()` methods.

### **Example: Naming Threads**
```java
class NamingThreadExample extends Thread {
    public void run() {
        System.out.println("Thread running: " + Thread.currentThread().getName());
    }
    public static void main(String[] args) {
        NamingThreadExample t1 = new NamingThreadExample();
        NamingThreadExample t2 = new NamingThreadExample();
        
        t1.setName("FirstThread");
        t2.setName("SecondThread");
        
        t1.start();
        t2.start();
    }
}
```
---
## **4. Daemon Threads in Java**
Daemon threads run in the background and provide support to non-daemon threads. They automatically terminate when all user threads finish execution.

### **Example: Creating a Daemon Thread**
```java
class DaemonThreadExample extends Thread {
    public void run() {
        if(Thread.currentThread().isDaemon()) {
            System.out.println("Daemon thread executing...");
        } else {
            System.out.println("User thread executing...");
        }
    }
    public static void main(String[] args) {
        DaemonThreadExample t1 = new DaemonThreadExample();
        DaemonThreadExample t2 = new DaemonThreadExample();
        
        t1.setDaemon(true);
        
        t1.start();
        t2.start();
    }
}
```
---
## **5. Thread Safety in Java**
Thread safety ensures that multiple threads can access shared resources without causing data inconsistency.

### **Ways to Achieve Thread Safety:**
1. **Synchronization**
2. **Using `volatile` keyword**
3. **Using `Atomic` variables**
4. **Using `ReentrantLock`**
5. **Using Concurrent Collections**

### **Example: Synchronization for Thread Safety**
```java
class SharedResource {
    synchronized void printNumbers(int n) {
        for (int i = 1; i <= 5; i++) {
            System.out.println(n * i);
            try { Thread.sleep(500); } catch (Exception e) {}
        }
    }
}
class MyThread1 extends Thread {
    SharedResource obj;
    MyThread1(SharedResource obj) { this.obj = obj; }
    public void run() { obj.printNumbers(5); }
}
class MyThread2 extends Thread {
    SharedResource obj;
    MyThread2(SharedResource obj) { this.obj = obj; }
    public void run() { obj.printNumbers(10); }
}
class ThreadSafetyExample {
    public static void main(String args[]) {
        SharedResource obj = new SharedResource();
        MyThread1 t1 = new MyThread1(obj);
        MyThread2 t2 = new MyThread2(obj);
        t1.start();
        t2.start();
    }
}
```
---
## **6. Thread Pools in Java**
Thread pools manage multiple worker threads efficiently, reducing the overhead of creating and destroying threads.

### **Using `ExecutorService` to Create a Thread Pool**
```java
import java.util.concurrent.ExecutorService;
import java.util.concurrent.Executors;

class Task implements Runnable {
    public void run() {
        System.out.println("Task executed by: " + Thread.currentThread().getName());
    }
}
class ThreadPoolExample {
    public static void main(String[] args) {
        ExecutorService executor = Executors.newFixedThreadPool(3);
        for (int i = 0; i < 5; i++) {
            executor.execute(new Task());
        }
        executor.shutdown();
    }
}
```
---
## **7. Summary of Java Multithreading Concepts**
- The **main thread** is the entry point of execution.
- **Thread priority** determines the scheduling preference.
- **Threads can be named** using `setName()` and `getName()`.
- **Daemon threads** run in the background and terminate when user threads complete.
- **Thread safety** ensures consistency using synchronization, locks, and atomic variables.
- **Thread pools** optimize performance by managing multiple threads efficiently.

---
# Java Streams and Lambda Expressions - Detailed Explanation

Java Streams and Lambda Expressions are powerful features introduced in Java 8 that enable functional-style programming and improve code readability and efficiency.

---
## **1. Java Streams**
Java Streams provide a way to process sequences of data declaratively, making code more readable and maintainable. They support operations like filtering, mapping, sorting, and reducing.

### **Key Features of Streams:**
- **Functional-style processing**
- **Lazy evaluation**
- **Parallel processing capability**
- **Immutable and stateless**

### **Creating a Stream**
Streams can be created from various sources like collections, arrays, or I/O channels.

#### **Example: Creating a Stream from a List**
```java
import java.util.Arrays;
import java.util.List;
import java.util.stream.Stream;

class StreamExample {
    public static void main(String[] args) {
        List<String> names = Arrays.asList("Alice", "Bob", "Charlie");
        Stream<String> stream = names.stream();
        stream.forEach(System.out::println);
    }
}
```

---
## **2. Stream Operations**
Stream operations are divided into two types:
1. **Intermediate Operations** (return another stream, allowing chaining)
2. **Terminal Operations** (consume the stream and produce a result)

### **Common Intermediate Operations:**
| Operation | Description |
|-----------|-------------|
| `filter(Predicate<T>)` | Selects elements based on a condition |
| `map(Function<T,R>)` | Transforms elements |
| `sorted()` | Sorts the stream elements |
| `distinct()` | Removes duplicates |
| `limit(n)` | Limits the number of elements |

### **Common Terminal Operations:**
| Operation | Description |
|-----------|-------------|
| `forEach(Consumer<T>)` | Iterates through elements |
| `collect(Collector<T>)` | Converts stream to a collection |
| `count()` | Counts the elements |
| `reduce(BinaryOperator<T>)` | Reduces elements to a single value |

#### **Example: Using Stream Operations**
```java
import java.util.Arrays;
import java.util.List;

class StreamOperationsExample {
    public static void main(String[] args) {
        List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);
        numbers.stream()
               .filter(n -> n % 2 == 0)
               .map(n -> n * n)
               .forEach(System.out::println);
    }
}
```
### **Output:**
```
4
16
36
64
100
```

---
## **3. Lambda Expressions in Java**
Lambda expressions are a way to write anonymous methods concisely. They enable functional programming by allowing functions to be passed as parameters.

### **Syntax of Lambda Expressions:**
```java
(parameters) -> expression
```
OR
```java
(parameters) -> { statements; }
```

### **Example: Using Lambda Expressions**
```java
interface MathOperation {
    int operation(int a, int b);
}

class LambdaExample {
    public static void main(String[] args) {
        MathOperation addition = (a, b) -> a + b;
        System.out.println("Sum: " + addition.operation(10, 5));
    }
}
```
### **Output:**
```
Sum: 15
```

---
## **4. Functional Interfaces and Lambda Expressions**
A functional interface has only one abstract method and can be used with lambda expressions.

### **Common Functional Interfaces in Java:**
| Interface | Method Signature | Description |
|------------|-----------------|-------------|
| `Predicate<T>` | `boolean test(T t)` | Evaluates a condition |
| `Function<T, R>` | `R apply(T t)` | Transforms an input to an output |
| `Consumer<T>` | `void accept(T t)` | Performs an action on input |
| `Supplier<T>` | `T get()` | Supplies values |

#### **Example: Using Predicate with Lambda**
```java
import java.util.function.Predicate;

class PredicateExample {
    public static void main(String[] args) {
        Predicate<Integer> isEven = n -> n % 2 == 0;
        System.out.println(isEven.test(10)); // true
        System.out.println(isEven.test(15)); // false
    }
}
```

---
## **5. Method References in Java**
Method references provide a shorthand for lambda expressions when a method already exists.

### **Types of Method References:**
1. **Static Method Reference** (`ClassName::staticMethod`)
2. **Instance Method Reference** (`object::instanceMethod`)
3. **Constructor Reference** (`ClassName::new`)

#### **Example: Using Method Reference**
```java
import java.util.Arrays;
import java.util.List;

class MethodReferenceExample {
    public static void main(String[] args) {
        List<String> names = Arrays.asList("Alice", "Bob", "Charlie");
        names.forEach(System.out::println);
    }
}
```

---
## **6. Stream Parallel Processing**
Java allows parallel execution of streams to improve performance using `parallelStream()`.

#### **Example: Parallel Stream Processing**
```java
import java.util.Arrays;
import java.util.List;

class ParallelStreamExample {
    public static void main(String[] args) {
        List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);
        numbers.parallelStream().forEach(System.out::println);
    }
}
```

---
## **7. Summary of Java Streams and Lambda Expressions**
- **Streams** simplify processing of collections using functional-style operations.
- **Lambda expressions** provide a concise way to represent functions.
- **Functional interfaces** enable passing behavior as parameters.
- **Method references** make code cleaner and more readable.
- **Parallel streams** leverage multi-core processors for performance improvement.
---
# Java I/O (Input and Output) - Detailed Explanation

Java provides a rich set of I/O (Input and Output) classes and methods that help in handling files, reading and writing data, and performing other I/O operations efficiently. The `java.io` package is the primary API for I/O in Java.

---
## **1. Java I/O Streams**
Java uses **streams** to perform input and output operations. A stream is a sequence of data that flows from a source to a destination.

### **Types of Streams:**
1. **Byte Streams** (used for binary data)
   - `InputStream` (read bytes)
   - `OutputStream` (write bytes)
2. **Character Streams** (used for text data)
   - `Reader` (read characters)
   - `Writer` (write characters)

### **Byte vs. Character Streams:**
| Feature | Byte Stream (`InputStream`, `OutputStream`) | Character Stream (`Reader`, `Writer`) |
|---------|----------------------------------|---------------------------------|
| Data Type | Handles raw binary data | Handles textual data (characters) |
| Example | FileInputStream, FileOutputStream | FileReader, FileWriter |
| Encoding | No character encoding support | Supports character encoding |

---
## **2. Byte Stream Classes**
Byte streams handle binary data like images, videos, and audio files.

### **Reading from a File using FileInputStream**
```java
import java.io.FileInputStream;
import java.io.IOException;

class ByteStreamReadExample {
    public static void main(String[] args) {
        try (FileInputStream fis = new FileInputStream("example.txt")) {
            int i;
            while ((i = fis.read()) != -1) {
                System.out.print((char) i);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

### **Writing to a File using FileOutputStream**
```java
import java.io.FileOutputStream;
import java.io.IOException;

class ByteStreamWriteExample {
    public static void main(String[] args) {
        try (FileOutputStream fos = new FileOutputStream("example.txt")) {
            String text = "Hello, Java I/O!";
            fos.write(text.getBytes());
            System.out.println("Data written successfully.");
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

---
## **3. Character Stream Classes**
Character streams handle text data efficiently.

### **Reading from a File using FileReader**
```java
import java.io.FileReader;
import java.io.IOException;

class CharacterStreamReadExample {
    public static void main(String[] args) {
        try (FileReader fr = new FileReader("example.txt")) {
            int i;
            while ((i = fr.read()) != -1) {
                System.out.print((char) i);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

### **Writing to a File using FileWriter**
```java
import java.io.FileWriter;
import java.io.IOException;

class CharacterStreamWriteExample {
    public static void main(String[] args) {
        try (FileWriter fw = new FileWriter("example.txt")) {
            fw.write("Hello, Java Character Stream!");
            System.out.println("Data written successfully.");
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

---
## **4. Buffered Streams**
Buffered streams improve performance by reducing the number of disk accesses.

### **Using BufferedReader to Read a File Efficiently**
```java
import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;

class BufferedReaderExample {
    public static void main(String[] args) {
        try (BufferedReader br = new BufferedReader(new FileReader("example.txt"))) {
            String line;
            while ((line = br.readLine()) != null) {
                System.out.println(line);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

### **Using BufferedWriter to Write a File Efficiently**
```java
import java.io.BufferedWriter;
import java.io.FileWriter;
import java.io.IOException;

class BufferedWriterExample {
    public static void main(String[] args) {
        try (BufferedWriter bw = new BufferedWriter(new FileWriter("example.txt"))) {
            bw.write("Hello, Buffered Writer!");
            System.out.println("Data written successfully.");
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

---
## **5. Serialization and Deserialization**
Serialization is the process of converting an object into a byte stream, and deserialization is converting it back into an object.

### **Example: Serializing an Object**
```java
import java.io.FileOutputStream;
import java.io.IOException;
import java.io.ObjectOutputStream;
import java.io.Serializable;

class Student implements Serializable {
    private static final long serialVersionUID = 1L;
    String name;
    int age;
    
    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }
}

class SerializationExample {
    public static void main(String[] args) {
        try (ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream("student.ser"))) {
            Student student = new Student("John", 22);
            oos.writeObject(student);
            System.out.println("Object serialized successfully.");
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

---
## **6. Summary of Java I/O**
- **Byte Streams** (`FileInputStream`, `FileOutputStream`) for binary data.
- **Character Streams** (`FileReader`, `FileWriter`) for text data.
- **Buffered Streams** (`BufferedReader`, `BufferedWriter`) for performance.
- **Serialization** converts objects into a byte stream.
- **Deserialization** reconstructs objects from a byte stream.

---
# Java Synchronization - Detailed Explanation

Synchronization in Java is a mechanism that helps prevent multiple threads from accessing shared resources simultaneously, ensuring data consistency and avoiding race conditions.

---
## **1. What is Synchronization?**
When multiple threads try to modify shared resources concurrently, it can lead to inconsistent results. Synchronization ensures that only one thread accesses the critical section at a time.

### **Why is Synchronization Needed?**
- Prevents data inconsistency
- Avoids race conditions
- Ensures thread safety

---
## **2. Types of Synchronization in Java**
### **1. Process Synchronization**
   - Managed by the operating system.
   - Uses mechanisms like semaphores and monitors.

### **2. Thread Synchronization**
   - Handled at the thread level in Java.
   - Uses `synchronized` keyword, `Lock` interface, and atomic variables.

---
## **3. Synchronized Blocks and Methods**
### **Synchronized Method**
A method declared with the `synchronized` keyword allows only one thread to execute it at a time.

#### **Example: Synchronized Method**
```java
class SharedResource {
    synchronized void display(String message) {
        for (int i = 0; i < 5; i++) {
            System.out.println(message + " - " + i);
            try {
                Thread.sleep(500);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
    }
}

class MyThread extends Thread {
    SharedResource resource;
    String message;

    MyThread(SharedResource resource, String message) {
        this.resource = resource;
        this.message = message;
    }

    public void run() {
        resource.display(message);
    }
}

class SynchronizedMethodExample {
    public static void main(String[] args) {
        SharedResource resource = new SharedResource();
        MyThread t1 = new MyThread(resource, "Thread 1");
        MyThread t2 = new MyThread(resource, "Thread 2");
        t1.start();
        t2.start();
    }
}
```

### **Synchronized Block**
Instead of synchronizing the whole method, we can synchronize only a specific block of code.

#### **Example: Synchronized Block**
```java
class SharedResource {
    void display(String message) {
        synchronized (this) {
            for (int i = 0; i < 5; i++) {
                System.out.println(message + " - " + i);
                try {
                    Thread.sleep(500);
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }
    }
}
```

---
## **4. Static Synchronization**
When a static method is synchronized, it locks the class object instead of the instance.

#### **Example: Static Synchronization**
```java
class SharedResource {
    synchronized static void display(String message) {
        for (int i = 0; i < 5; i++) {
            System.out.println(message + " - " + i);
            try {
                Thread.sleep(500);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
    }
}
```

---
## **5. Inter-thread Communication**
Java provides `wait()`, `notify()`, and `notifyAll()` methods to allow threads to communicate with each other efficiently.

#### **Example: wait() and notify()**
```java
class SharedResource {
    synchronized void produce() {
        System.out.println("Producer is producing...");
        try {
            wait();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        System.out.println("Resumed production!");
    }

    synchronized void consume() {
        System.out.println("Consumer is consuming...");
        notify();
    }
}
```

---
## **6. Lock Interface (java.util.concurrent.locks)**
Java provides the `Lock` interface to implement synchronization in a more flexible way than the `synchronized` keyword.

#### **Example: Using ReentrantLock**
```java
import java.util.concurrent.locks.Lock;
import java.util.concurrent.locks.ReentrantLock;

class SharedResource {
    private final Lock lock = new ReentrantLock();

    void display(String message) {
        lock.lock();
        try {
            for (int i = 0; i < 5; i++) {
                System.out.println(message + " - " + i);
                Thread.sleep(500);
            }
        } catch (InterruptedException e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
        }
    }
}
```

---
## **7. Thread Synchronization Techniques**
| Technique | Description |
|-----------|-------------|
| `synchronized` keyword | Locks methods or blocks to ensure only one thread can access them at a time. |
| `wait()`, `notify()`, `notifyAll()` | Enables inter-thread communication. |
| `Lock` interface | Provides more flexibility than `synchronized`. |
| `volatile` keyword | Ensures visibility of changes to variables across threads. |
| `Atomic Variables` | Provides lock-free thread-safe operations. |

---
## **8. Summary of Java Synchronization**
- Synchronization prevents data corruption in multi-threaded environments.
- Use `synchronized` methods or blocks to control thread access.
- Static synchronization locks the class instead of an object.
- `wait()`, `notify()`, and `notifyAll()` help in thread communication.
- `Lock` interface provides an alternative to `synchronized`.

---
# Java Memory Allocation and Garbage Collection - Detailed Explanation

Java handles memory management through automatic memory allocation and garbage collection. Understanding these concepts ensures efficient resource usage and prevents memory leaks.

---
## **1. Java Memory Allocation**
Java memory is divided into different areas to optimize performance and manage objects efficiently.

### **Memory Areas in Java**
| Memory Area | Description |
|------------|-------------|
| **Heap Memory** | Stores objects and class instances. Managed by the Garbage Collector. |
| **Stack Memory** | Stores method calls, local variables, and references to objects. Each thread has its own stack. |
| **Method Area** | Stores class metadata, static variables, and method code. Part of the heap. |
| **Program Counter (PC) Register** | Keeps track of the currently executing instruction. |
| **Native Method Stack** | Stores native method calls used in Java programs. |

---
## **2. Heap Memory Structure**
Heap memory is divided into different generations for efficient garbage collection:

| Heap Generation | Description |
|----------------|-------------|
| **Young Generation** | Stores newly created objects. Further divided into **Eden Space** and **Survivor Spaces (S0, S1)**. |
| **Old Generation (Tenured)** | Stores long-lived objects that survive multiple garbage collection cycles. |
| **Permanent Generation (Metaspace in Java 8+)** | Stores class metadata, method information, and static variables. |

### **Diagram Representation of Memory Areas:**
```
+----------------------+  
| Method Area          |  
| Static Variables     |  
+----------------------+  
| Heap Memory         |  
| - Young Generation  |  
|   - Eden Space      |  
|   - Survivor S0, S1|  
| - Old Generation    |  
+----------------------+  
| Stack Memory        |  
| - Method Call Stack |  
| - Local Variables   |  
+----------------------+  
```

---
## **3. Java Garbage Collection**
Garbage collection in Java automatically reclaims memory occupied by unreachable objects.

### **Types of Garbage Collectors**
| Garbage Collector | Description |
|------------------|-------------|
| **Serial GC** | Single-threaded, suitable for small applications. Uses a simple mark-and-sweep algorithm. |
| **Parallel GC** | Uses multiple threads to speed up garbage collection. Best for multi-core processors. |
| **CMS (Concurrent Mark-Sweep) GC** | Minimizes pause times by collecting garbage concurrently with the application. |
| **G1 (Garbage First) GC** | Default GC in Java 9+. Splits the heap into regions for efficient memory management. |
| **ZGC (Z Garbage Collector)** | Low-latency garbage collector introduced in Java 11. Handles large heaps efficiently. |
| **Shenandoah GC** | Reduces GC pause times by performing concurrent operations. |

---
## **4. How Garbage Collection Works**
Garbage collection follows these steps:
1. **Mark Phase** – Identifies reachable and unreachable objects.
2. **Sweep Phase** – Removes unreachable objects.
3. **Compact Phase** – Rearranges memory to avoid fragmentation (optional in some collectors).

### **Example: Triggering Garbage Collection Manually**
```java
class GarbageCollectionExample {
    protected void finalize() throws Throwable {
        System.out.println("Garbage Collector is running...");
    }
    public static void main(String[] args) {
        GarbageCollectionExample obj = new GarbageCollectionExample();
        obj = null; // Making the object eligible for garbage collection
        System.gc(); // Requesting garbage collection
    }
}
```

> **Note:** Calling `System.gc()` is a request, not a guarantee for garbage collection execution.

---
## **5. Memory Leaks in Java and How to Avoid Them**
Even though Java has automatic garbage collection, memory leaks can still occur in certain scenarios:

### **Common Causes of Memory Leaks:**
- **Static Collections:** Storing objects in static collections without proper removal.
- **Unclosed Resources:** Not closing file streams, database connections, etc.
- **Listener References:** Not removing listeners from components.
- **Thread Local Variables:** Holding references to large objects.

### **Preventing Memory Leaks:**
- Use **try-with-resources** for closing resources automatically.
- Remove unnecessary references (e.g., `nullify` objects when no longer needed).
- Use profiling tools like **JVisualVM** and **Eclipse MAT** to detect memory leaks.

---
## **6. Finalization and Weak References**
### **Finalization (`finalize()` method)**
Java provides a `finalize()` method that gets called before an object is garbage collected. However, it is not recommended due to its unpredictable execution.

### **Weak References**
Java provides different types of references to help with memory management:

| Reference Type | Description |
|---------------|-------------|
| **Strong Reference** | Default type. Prevents garbage collection. |
| **Weak Reference** | Allows GC to reclaim memory when needed. |
| **Soft Reference** | Retained longer than weak references, but collected when memory is low. |
| **Phantom Reference** | Used for cleanup actions before object removal. |

#### **Example: Using Weak References**
```java
import java.lang.ref.WeakReference;

class Example {
    public static void main(String[] args) {
        String strongRef = new String("Strong Reference");
        WeakReference<String> weakRef = new WeakReference<>(strongRef);
        strongRef = null; // Eligible for GC
        System.gc();
        System.out.println("Weak Reference Value: " + weakRef.get());
    }
}
```

---
## **7. Summary of Java Memory Management**
- **Heap Memory:** Stores objects, divided into Young and Old Generations.
- **Stack Memory:** Stores local variables and method calls.
- **Garbage Collection:** Automatically reclaims unused objects.
- **Types of GC:** Serial, Parallel, CMS, G1, ZGC, Shenandoah.
- **Avoid Memory Leaks:** Use proper memory management techniques.
- **Weak References:** Help manage memory efficiently without strong ownership.


