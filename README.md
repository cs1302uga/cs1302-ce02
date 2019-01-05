# ce02 Command Line Compilation and Packages

This exercise is designed to introduce text editors and compiling java code organized in packages on a Unix system

## Prerequisite Knowledge
Emacs How-To: https://www.digitalocean.com/community/tutorials/how-to-use-the-emacs-editor-in-linux

CSCI 1302 Package Tutorial: https://github.com/cs1302uga/cs1302-tutorials/blob/master/packages.md

Emacs Reference Card: https://www.gnu.org/software/emacs/refcards/pdf/refcard.pdf
Vi Reference Guide: https://www.ks.uiuc.edu/Training/Tutorials/Reference/virefcard.pdf

## Questions

In your notes, clearly answer the following questions. These instructions assume that you are logged into the nike server.

1. Launch your terminal emulator and create the subdirectory structure seen below. What single command can be used to 
   create all of these directories at once?

   ```
   exercise2
    |--- src
          |--- cs1302
                |--- example
   ```

1. Navigate to the default package for source code. Within this directory, create a file called `Hello.java`. Within this file, write 
   a basic java program (using your favorite command-line text editor) to read in the user's name and then output "Hello, \<user\>" with 
   their name instead of \<user\>.  Your program should work **without any import statements**.  What is the line of java code to 
   instantiate a `Scanner` object without importing the class?

1. Compile and run your code directly from the default package.  In which directory is the compiled code at this point?  

   Once you are confident that it is working, remove the compiled code.

1. Move the `Hello.java` file into the `cs1302.example` package.  What two things must be done to accomplish this?

1. For better organization, let's separate the source code from the compiled code.  From the `exercise2` directory, add a subdirectory 
   called `bin`. This folder will be the default package for our compiled code. What is the single command to compile `Hello.java` and 
   place the compiled code in the `bin` directory?

1. From the `exercise2` directory, what is the single command to run the `Hello` java program?

1. From your home directory (not `exercise2`), what is the single command to run the `Hello` java program? The correct answer will be
different for each group.

    **CHECKPOINT**
    
1. Create a `cs1302.utility` package directory. Add a new java file called `MyMethods.java` to this package. Add a single, static 
   method to `MyMethods.java` which takes two integers as parameters and returns the max of the two.  What is the exact first line of
   code in `MyMethods.java`?

1. Assuming your present working directory is still `exercise2`, what is the command to compile `MyMethods.java` and place the byte code
   in the `bin` directory?  Look in the `bin` directory now that you've compiled both `Hello.java` and `MyMethods.java`.  Notice the 
   directory hierarchy that was automatically created.

1. Now, modify your `Hello.java` file.  Have it print out the maximum of two values input by the user.  Use the max method from your
   `MyMethods.java` utility. What is the line of code to call this method?  Assume you have **no import statements** in `Hello.java`.
  
1. What is the line to compile the `Hello.java` file from the `exercise2` directory and place the compiled code into `bin`? Note: there
   is now a dependency in `Hello.java`.  It relies on the code from `MyMethods`, so the compiler needs to know where to find that class.

1. Now, add the import statement for `MyMethods` and remove the fully qualified name from `Hello.java`. Rerun your code to make sure
   it is working.

    **CHECKPOINT**

1. Add a README.txt file in the `exercise2` folder containing the first and last names of all group members (one full name per line).

1. Change directories to the parent of `exercise2` (so, `cd..` from `exercise2`). We will use the `tar` command to combine our directory
   hierarchy into a single file for submission.  To do this, execute the command:
   
   ```
   tar -cf exercise2.tar exercise2/
   ```
1. List the contents of your directory and make sure you see `exercise2.tar`.  Now, to make sure this tar file contains all of the work 
   you just did, list all of its contents with the command:
   
   ```
   tar -tf exercise2.tar
   ```
1. Now, to make this file smaller, we will compress it with gzip.  Execute the command:
   ```
   gzip exercise2.tar
   ```
1. List the contents of your directory and make sure you see `exercise2.tar.gz` instead of `exercise2.tar`. Now, submit this file using
   the following command.  **Note:** You must be on nike to submit.
   ```
   submit exercise2.tar.gz cs1302a
   ```

    **CHECKPOINT**

<hr/>

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-nc-nd/4.0/)

<small>
Copyright &copy; Michael E. Cotterell, Brad Barnes, and the University of Georgia.
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a> to students and the public.
The content and opinions expressed on this Web page do not necessarily reflect the views of nor are they endorsed by the University of Georgia or the University System of Georgia.
</small>

