# Simple Shell
This project is the final project in the first trimester of the ALX SE Program. It is the consolidation of everything we learned in the quarter about System engineering & DevOps and Low-level programming & Algorithm.
Using C programming language, we develop our own Shell.

### Description
The shell is a command-line interpreter or shell that provides a command line user interface for Unix-like operating systems. The shell is both an interactive command language and a scripting language, and is used by the operating system to control the execution of the system using shell scripts.

___
### Installation
You can install the simple shell cloning this repo:
```sh
$ git clone https://github.com/andreammgcol/simple_shell.git
```
Next you can compile the files with this command:
```sh
$ gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
```
finally you can run our Shell writing:
```sh
./hsh
```
### Output Examples
```sh
vagrant@vagrant-ubuntu-trusty-64:~/simple_shell$ ./hsh
($) ls -l
total 72
-rw-rw-r-- 1 vagrant vagrant  1054 Nov 26 01:42 builtin_commands.c
drwxrwxr-x 3 vagrant vagrant  4096 Nov 26 01:42 concepts
-rw-rw-r-- 1 vagrant vagrant   890 Nov 26 01:42 counters.c
-rw-rw-r-- 1 vagrant vagrant  1940 Nov 26 01:42 exec.c
-rw-rw-r-- 1 vagrant vagrant   372 Nov 26 01:42 frees.c
-rwxrwxr-x 1 vagrant vagrant 23170 Nov 26 01:43 hsh
-rw-rw-r-- 1 vagrant vagrant   876 Nov 26 01:42 main.c
-rw-rw-r-- 1 vagrant vagrant   812 Nov 26 01:41 README.md
-rw-rw-r-- 1 vagrant vagrant   304 Nov 26 01:42 remove_new_line.c
-rw-rw-r-- 1 vagrant vagrant   786 Nov 26 01:42 shell.h
-rw-rw-r-- 1 vagrant vagrant   253 Nov 26 01:42 signal_handler.c
-rw-rw-r-- 1 vagrant vagrant   606 Nov 26 01:42 tokenize.c
-rw-rw-r-- 1 vagrant vagrant  1041 Nov 26 01:42 utilities.c
($)
```
```sh
Holbertons-iMac-9:simple_shell holberton$ ./hsh 
($) pwd
/Users/holberton/simple_shell
```
```sh
($) cat signal_handler.c
#include "shell.h"

/**
  * signal_handler - Handles the signals
  * @sig_id: The identifier of the signal to handle
  *
  * Return: Nothing to returns
  */
void signal_handler(int sig_id)
{
	if (sig_id == SIGINT)
		write(STDOUT_FILENO, "\n($) ", 5);
}
($)
```

### Built with
This project was built and development with:
- `C programming language:` is a general-purpose, procedural computer programming language supporting structured programming, lexical variable scope, and recursion, while a static type system prevents unintended operations.
- `GitBash:` is an application for Microsoft Windows environments which provides an emulation layer for a Git command line experience. 
- `Ubuntu 14.04 LTS:` Operating system tester and working.

- `GCC:` GNU Compiler version 4.8.4
# Authors
- Etiene Francis Okokon - Development and documentation
- Issa Issa Taiwo - Development and documentation
