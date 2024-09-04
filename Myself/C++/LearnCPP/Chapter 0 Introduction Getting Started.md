Why were Languages made
Due to portability issues of Machine code Assembly Language was invented

One layer of abstraction from the CPU 

Challenging still to read entire program

Assembly still not portable due to different commands

#High_Level_Languages was invented

Two ways to run Languages #Compile or #Interpret

C++ uses Compiler 


![[Screenshot 2024-09-03 at 3.04.00 PM.png]]

Interpreter

![[Screenshot 2024-09-03 at 3.04.29 PM.png]]
High Level languages 
Easier to read
Less commands
Can be run on multiple systems

Intro to C/C++

#C Language was developed in 1972 Dennis Ritchie

C was applied to UNIX instead of Assembly allowing for great portabiity

#Cplusplus was developed by Bjarne Stroustrup in 1979 somewhat of a superset of C

Offering Classes for Object Oriented Programming

5 Updates #Cplusplus11 #Cplusplus14 #Cplusplus17 #Cplusplus20 #Cplusplus23 

These were called Language Standards or Specifications named after the year of release

The Motto is "trust the programmer" for both these languages. True freedom, but scary. 

C++ excels in situations where high performance and precise control over memory and other resources is needed. Here are a few common types of applications that most likely would be written in C++:

- Video games
- Real-time systems (e.g. for transportation, manufacturing, etc…)
- High-performance financial applications (e.g. high frequency trading)
- Graphical applications and simulations
- Productivity / office applications
- Embedded software
- Audio and video processing
- Artificial intelligence and neural networks

Introduction to C++ Development:
How does C++ get Developed?
![[Screenshot 2024-09-03 at 3.22.52 PM.png]]

First define the What


Then go for how: 
Think before you code! 

Various studies have shown that on complex software systems, only 10-40% of a programmer’s time is actually spent writing the initial program. The other 60-90% is spent on maintenance, which can consist of **debugging** (removing bugs), updates to cope with changes in the environment (e.g. to run on a new OS version), enhancements (minor changes to improve usability or capability), or internal improvements (to increase reliability or maintainability)[1](https://web.archive.org/web/20120313070806/http://users.jyu.fi/~koskinen/smcosts.htm).

Write The program:
First have knowledge of the language  and use a text editor or code editor(More advanced)

Some advantages of #code_editors
1. Line numbering. Line numbering is useful when the compiler gives us an error, as a typical compiler error will state: _some error code/message, line 64_. Without an editor that shows line numbers, finding line 64 can be a real hassle.
2. Syntax highlighting and coloring. Syntax highlighting and coloring changes the color of various parts of your program to make it easier to identify the different components of your program.
3. An unambiguous, fixed-width font (often called a “monospace font”). Non-programming fonts often make it hard to distinguish between the number 0 and the letter O, or between the number 1, the letter l (lower case L), and the letter I (upper case i). A good programming font will ensure these symbols are visually differentiated in order to ensure one isn’t accidentally used in place of the other. All code editors should have this enabled by default, but a standard text editor might not. Using a fixed-width font (where all symbols have the same width) makes it easier to properly format and align your code.

The first Source File is always main.cpp


Compiling Source code
Compiler goes through each .cpp file

First checks for errors

Second, compiler transaltes C++ code into machine language instructions that are stored in opbject file 

Typically the object files are name.o or name.obj same as cpp file name
![[Screenshot 2024-09-03 at 3.36.05 PM.png]]

Linker comes in and combines all object files and produces an executable file 

First reads in each object files and ensures validity 

All cross file dependency are resolved using one . for example: .cpp and used another cpp in that file

Link library files precokmpiled code that been packaged to reuse in other programs

C++ comes with a library called C++ standard Library
It contains handy things like iosstream 

C++ links this library automatically 
![[Screenshot 2024-09-03 at 3.39.57 PM.png]]
Executable will be at the end of this 

Building is often used to refer to this process

Testing and debugging is the last step 

