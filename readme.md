# Generic Linked List in C

* Includes a number of common linked list functions
* Node values are void pointers to enable the implementation to be generic
* Attempting to access an invalid index will throw a fatal error
* Undefined behaviour will occur if a null pointer is passed into a function expecting `linkedList*`
* See  `linkedListTest.c` for an example of how to use some of the functions

## Building the test

* Build by navigating into the directory where the Makefile is located and run `make test` to build a test demo
* Run the resulting executable with `./linkedListTest`
* Run `make leakCheck` to build a test and automatically run valgrind on it

## Installation to system libraries

* Automated installation below is only available for macOS
* Run: `make install` from within the directory where the Makefile is located
* Run: `make uninstall` to remove previously installed files
* Include in a program (eg `programName.c`) with `#include <linkedlist.h>`
* Compile with `gcc programName.c -lGenericStructures -o programName`
