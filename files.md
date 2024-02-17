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
