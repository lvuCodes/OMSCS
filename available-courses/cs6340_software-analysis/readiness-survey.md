# CS 6340 — Readiness Assessment

Source: [Readiness Assessment (Google Doc)](https://docs.google.com/document/d/1keAPPrAYixtMIj7wcWqcpoiOHmSYYmVIF0LOxyOn8ow/edit). This assessment helps determine specific skills and concepts to learn or re-familiarize with before starting the course. You do not need to master every one, but you should have command of the majority. Some skills can be picked up along the way, but covering them all is difficult (especially in shortened summer semesters). Instructors and TAs have limited capability to assist with these tasks, and they are not explicitly covered in video lessons.

In this course, you will use a variety of tools implemented in different programming languages to generate useful facts about a program's behavior and analyze them. You will learn about the tools and their theoretical underpinnings, but it is assumed that you are already familiar with basic concepts in computer science and mathematics, as well as the use of various tools/commands in a UNIX-like environment.

## Using a Container or Virtual Machine

Assignments are completed in a Docker container (preferred; required for M-series Macs) or on a Virtual Machine provided by the teaching staff. The container provides a common operating platform that is also used for grading, ensuring code behaves the same way when graded. You should be comfortable running and using either a Docker image or a [VirtualBox](https://www.virtualbox.org/wiki/VirtualBox) VM, including importing a VM from a `.ova` file and adjusting VM settings (network, memory allocation, etc.). If you are unfamiliar with containerization or virtualization, see [Virtualization](https://en.wikipedia.org/wiki/Virtualization).

## Navigating a UNIX-like Environment

All assignments assume a UNIX-like environment. You should be comfortable browsing folders and executing basic commands from a UNIX command prompt. In particular, you should fully understand the difference between these two paths:

- `tmp`
- `/tmp`

**Sample task:** Using just a command prompt in a UNIX-like environment (such as Linux or macOS), create a new folder, create a text file inside that folder, and change the file permissions to allow execution of that file (as would be needed if the file contained a shell script). Finally, create a ZIP archive of your folder and extract it to a different location to verify that it was correctly created.

## Understanding of Object-Oriented Programming

You should have a strong understanding of object-oriented programming concepts, and specifically how they are implemented in common languages like C/C++, Java, and Python.

**Sample task:** In both Java and C++, write a small program that exploits the power of inheritance, abstraction, encapsulation, and polymorphism. For example, create a code library with an abstract superclass `Organism` and create subclasses for the Animal Kingdom down to the Mammal Class.

## Using and Evaluating Data Structures in Code

You will perform analysis on common data structures such as trees, heaps, queues, and stacks. You should be able to write code in Java and C++ that uses common data structures.

**Sample task:** Using a high-level language such as Java or C++, write a class that builds a balanced binary tree out of an unsorted array of integer values. Then write a search function to determine if a specific value exists in the tree. Your search function should use an algorithm such as BFS (Breadth First Search) or DFS (Depth First Search) on the tree values and return false if the desired value does not exist in the tree.

Sample input array of values: `[26, 28, 76, 32, 4, 87, 42, 9, 12]`

## Using Pointers in C/C++

Some assignments require the use of pointer constructs to interact with objects and collections of objects, as well as pointer-specific operators like `&`, `*`, and `->`.

**Sample task:** You should be able to answer the following questions regarding pointer constructs:

1. What is the difference between passing by value and passing by reference?
2. Given an object `Foo`, how would you:
   1. Obtain a pointer to the object in C++?
   2. Using that pointer, access a public class member called `name`?
3. What does it mean for a pointer to be `NULL`?
4. What happens when you use the reference operator `&` on a `NULL` pointer?
5. What is the difference between an array of pointers to objects and an array of the same objects?
6. How can pointers be used with inherited and/or abstract classes?

## Debugging High-Level Code

Some tools explored in this class automatically generate test cases that find bugs in a provided application. You should be able to use a compile error or stack trace to figure out why a source file doesn't compile, and find and fix issues such as null pointer exceptions or invalid cast errors. As many applications analyzed are relatively simple, a high level of comfort debugging simple issues without the help of an IDE is recommended.

**Sample task:** Run the following Java program. Make sure that all code in the `main` method executes to produce correct results.

```java
public class test {
    public static void main(String[] args) {
        System.out.println("Add 1 + 2:");
        System.out.println("Result = " + add(1,2));
        System.out.println("Add 40 + 2:");
        System.out.println("Result = " + add(40,2));
        System.out.println("Multiply 3 x 4:");
        System.out.println("Result = " + multiply(3,4));
        System.out.println("Multiply 12 x 20:");
        System.out.println("Result = " + add(12,20));
        System.out.println("Done!")
    }

    public static int add(int a, int b) {
        Integer result = null;
        result += a;
        result += b;
        return result;
    }

    public static int multiply(int a, int b) {
        int result = -1;
        for (int i = 0; i < b; i++)
            result = add(result, a);
        return result;
    }
}
```

## Using Man Pages and Modifying Commands

Many software analysis tools require more knowledge of the tool than is provided in assignment instructions. You should be comfortable reading the documentation provided with tools and utilities. In particular, man pages give basic usage instructions and how to modify a command to accomplish different tasks.

**Sample task:** Use the `uniq` UNIX tool to take the following text (copy it into a text file) and remove duplicate lines.

```
The quick brown fox jumps over the lazy dog.
THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG.
The Quick Brown Fox Jumps Over The Lazy Dog.
My quick brown fox jumps over the lazy dog.
His quick brown fox jumps over the lazy dog.
The quick, brown fox jumps over the lazy dog.
The quick brown fox jumps over the lazy dog.
```

Modify your command to do the following:

1. Prefix each line by the number of occurrences of that line in the file
2. Skip comparing the first three characters on the line
3. Ignore the case of the characters in the comparison

Hint: use the `man` command to figure out the capabilities of `uniq`.

## Understanding of Random Distributions and Sampling

Some analysis and testing techniques exploit the power of randomness. While a thorough understanding of probability and statistics is not necessary, you should be familiar with the concepts of Random Distribution and Random Sampling, and be able to apply them to randomized algorithms and reason about the likelihood of a particular program behavior.

**Sample task:** Assume you are writing a program to randomly award a prize to contestants. Contestants enter a 32-bit unsigned integer at random. If the number entered is between 50 and 65 and divisible by 5, the contestant wins.

1. What is the likelihood that any given contestant will win?
2. Assuming the program handles one contestant per minute, how long should we expect the game to run before a contestant wins — minutes, hours, days, weeks, or months?
3. If the contestant enters the string "WIN" instead of an integer, what is the likelihood that the contestant will win?

## Working Knowledge of Code Build Processes

The primary focus of this course is software analysis. Software can be analyzed at various stages in its life cycle, including source code written by the programmer, an intermediate representation generated by a compiler or language toolchain, and the program's binary representation. While extensive knowledge of compilers, toolchains, and runtimes is not necessary, you should have a working knowledge of what happens to your code when you "build" it.

**Sample task:** You should be able to answer the following questions regarding code build processes:

1. What is the difference between high-level code, intermediate representation, assembly code, and machine language?
2. What is the difference between a compiled language and an interpreted language?
3. What happens to C/C++ code when you click "Build and Run" in an IDE?
4. What happens to Java code when you click "Build and Run" in an IDE?
