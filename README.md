# ce02 Command Line Compilation and Packages

This exercise is designed to introduce text editors and compiling java code organized in packages on a Unix system

## Prerequisite Knowledge
Emacs/Vi Reference Guide
Introduction to Java Packages: https://docs.oracle.com/javase/tutorial/java/package/index.html

**Might Need More Resources Here**

## Questions

In your notes, clearly answer the following questions. These instructions assume that you have setup
your local machine following the instructions linked to on eLC and the syllabus.

1. Launch your terminal emulator and create the following directory hierarchy: 'exercise2/src/cs1302/example'
   What single command can be used to create this directory structure?

2. Within the 'example' directory, create a file called 'Hello.java'. Inside of the file, write a basic java program 
   using your favorite text editor (emacs or vi).  `Hello.java` should read in the user's name (using Scanner) and then output
   "Hello, <user>" with their name instead of <user>.  Your program should work without any import statements (do not directly input
   the Scanner class).  How can you use Scanner without importing it?

3. Within the Hello.java file, write code to place this file in the 'cs1302.example' package.

4. From the 'exercise2' directory, make a directory called 'bin'. This folder will hold the byte code (.class files) for 
   our program.

5. From the 'exercise2' directory, what is a single command to compile the 'Hello.java' file and place the .class file in
   the 'bin' directory?

6. From the 'exercise2' directory, what is the single command to run the 'Hello' java program?

7. From your home directory (not 'exercise2'), what is the single command to run the 'Hello' java program?

* **CHECKPOINT**
8. Create a 'utility' package under the 'cs1302' package at the same level as 'example'.  In 'utility', create a 'Methods.java' file that    contains a single, static method which takes two integers as input and returns the max of the two.  What is the exact first line of
   code in this file? **Hint**: it should be a package specifier.

9. What is the command to compile 'Methods.java' and place the byte code in the 'bin' directory?  Look in the bin directory when you've
   compiled both 'Hello.java' and 'Methods.java'.  Notice the directory hierarchy that was automatically created.

10. Now, modify your 'Hello.java' file.  Have it print out the maximum of two values input by the user.  Use the max method from your 'Methods.java' utility. What is the line of code to call this method?  Assume you have no import statements in 'Hello.java'.
  
11. What is the line to compile the 'Hello.java' file?  Has compilation changed?


12. Now, add the import statement and remove the fully qualified name from the code.

* **CHECKPOINT**

11. Extend homework 2 to do the same thing using maven in exercise 3?  When you add the utility folder, it just figures everything out.       Good motivator for maven.  This exercise gets tough toward the end.  

12.

13.

14.

15.

* **CHECKPOINT**

16.

17.

18.

19.

20.

* **CHECKPOINT**

<hr/>

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-nc-nd/4.0/)

<small>
Copyright &copy; Michael E. Cotterell, Brad Barnes, and the University of Georgia.
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a> to students and the public.
The content and opinions expressed on this Web page do not necessarily reflect the views of nor are they endorsed by the University of Georgia or the University System of Georgia.
</small>

