File handling in C refers to the process of working with files in the C programming language. It involves performing various operations such as creating, opening, reading, writing and closing files.

-These files are declared in the <stdio.h> header file

Steps to processing a file:
1. Declare a file pointer variable.
2. open a file using fopen()
3. Process th file using the appropriate function.
4. close the file using fclose()

The general syntax to open a file:
FILE *ptr;
ptr = fopen("file_name", "mode");

standard streams: Refers to the default input and output channels associated with a running program which are:
1) standard input (stdin)
2) Standard ouptput (stdout)
3) Standard error (stderr)

*Standard input (stdin): Provides way for the program to receive input from the user or from another program. Keyboard input, input function like scanf() and fgets()

*Standard output: associated with the terminal/console and output functions like printf() and puts() write data to stdout.

*Standard error (stderr): Outputs error messages to the console using functions like fprintf() or perror()

* unlike stdout, stderror is typically unbuffered meaning the output is immediately displayed instead of being stored in a buffer.

##Functions.
1) fopen() - To open a file
2) getc() - Read a character from a file
3) putc() - write character into a file
4) getw() - Read integer from a file
5) putw() - Write an integer into a file
6) fclose() - To close a file
7) fprintf() - prints formatted output into a file
8) fcsanf() - Read formatted input from a file
9) fputs() - write a string from a file
10) fgets() - Read a string from a file
11) feof() - Detect end of file marker



##PROCESSES (PID - Process Identifier)
##Parent Process Identifier(PPID)

An instance of an executing program that has a unique ID

The pid_t data type is a signed integer type which is capable of representing a process ID.
/**
#include <unistd.h>
getpid(); //Takes no arguments, returns process id.
*/
get ppid() //returns the parent process id.
echo $$ //returns pid from the terminal
##CommandLine Arguments (argc and argv)

##Executing a program (with execve system call)

##Creating processes (with the fork system call)
System call fork() is used to create processes.
It takes no arguments.
It returns the pid of child in the parent 0 means success, -1 if unsuccessful.
It accepts no parameters.
* after a new child process is created, both processes will execute the next instruction following the fork() system call.

When the child exits, it returns back to the parent.

if parent has already exited before child returns, * the child gets stranded in what is called the orphan.
// Parent id of child process changes during execution to 1
//Child process is removed from process table after execution.


### Orphan process
This is a running whose parent terminated/exited.

## Init process
The parent of all processes, executed by the kernel during the booting of the system.
It has a pid of 1.

## Process Table
This is a data structure in the RAM of a computer that holds information about the processes currently being handled by the Os.

## Process Entry
This is created when the process is created by fork() system call.

##Suspending processes (with wait system call)
Helps prevent rise/creation of zombie states for child processes which normally occurs when child processes terminate before the parent process has terminated.

#Getline function



##File Information (with the stat system call)

##Environment (printenv, etc)
