# ALX Simple Shell Team Project

> This is an ALX collaboration project on Shell. We were asked to create a shel that works like the Bash shell. We will refer to our  shell as  *Balgbe**

## Project was completed using

- C language
- Shell
- Betty linter

## General Requirement for project
Allowed editors: vi, vim, emacs

All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89

All your files should end with a new line

A README.md file, at the root of the folder of the project is mandatory

Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl

Your shell should not have any memory leaks

No more than 5 functions per file

All your header files should be include guarded

Use system calls only when you need to (why?)

Write a README with the description of your project

You should have an AUTHORS file at the root of your repository, listing all individuals having contributed content to the repository. Format, see Docker



## Description ##

**Balgbe** is a simple UNIX command language interpreter that reads commands from either a file or standard input and executes them.

### How **Balgbe** works
* Prints a prompt and waits for a command from the user
* Creates a child process in which the command is checked
* Checks for built-ins, aliases in the PATH, and local executable programs
* The child process is replaced by the command, which accepts arguments
* When the command is done, the program returns to the parent process and prints the prompt
* The program is ready to receive a new command
* To exit: press Ctrl-D or enter "exit" (with or without a status)
* Works also in non interactive mode

### Compilation

`gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh`

### Invocation

Usage: **Balgbe**

To invoke **Balgbe**, compile all `.c` files in the repository and run the resulting executable.

**Balgbe** can be invoked both interactively and non-interactively. If **hsh** is invoked with standard input not connected to a terminal, it reads and executes received commands in order.

Example:
```
$ echo "echo 'hello'" | .Balgbe
'hello'
$
```

If **Balgbe** is invoked with standard input connected to a terminal (determined by [isatty](https://linux.die.net/man/3/isatty)(3)), an *interactive* shell is opened. When executing interactively, **hsh** displays the prompt `$ ` when it is ready to read a command.



### What we learned:
* How a shell works and finds commands
* Creating, forking and working with processes
* Executing a program from another program
* Handling dynamic memory allocation in a large program
* Pair programming and team work
* Building a test suite to check our own code


## Authors ##
Bala Sule
Damigbe
