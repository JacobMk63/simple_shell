#simple_shell
##Yakob Mengistu
###Project Descriptio: more details about the C - Simple Shell project.

The project involves implementing a basic command-line interface that can handle different commands and arguments. This can be achieved using the fork() and exec() system calls to create a new process and execute a command in that process.

The shell program should also handle input/output redirection using the < and > operators, as well as piping multiple commands together using the | operator. These functionalities can be implemented using the dup2() system call to redirect input/output streams and pipe() system call to create pipes between processes.

In addition, the shell should support built-in commands such as cd to change the current working directory, exit to terminate the shell, and help to display information about the shell and its commands.

Memory management is also an important aspect of the project. The shell program should allocate and free memory appropriately to avoid memory leaks and other issues.

Overall, the C - Simple Shell project can be a great way for students to learn about system calls, processes, input/output redirection, piping, memory management, and other important concepts in the C programming language.

Taks on this project

Simple shell 0.1

Simple shell 0.2 mandatory Simple shell 0.1 +

Handle command lines with arguments

Simple shell 0.3 mandatory Simple shell 0.2 +
Handle the PATH fork must not be called if the command doesn’t exist

Simple shell 0.4 mandatory Simple shell 0.3 +
Implement the exit built-in, that exits the shell Usage: exit You don’t have to handle any argument to the built-in exit

Simple shell 1.0 mandatory Simple shell 0.4 +
Implement the env built-in, that prints the current environment

Simple shell 0.1.1 #advanced Simple shell 0.1 +
Write your own getline function Use a buffer to read many chars at once and call the least possible the read system call You will need to use static variables You are not allowed to use getline You don’t have to:

be able to move the cursor

Simple shell 0.2.1 #advanced Simple shell 0.2 +
You are not allowed to use strtok

Simple shell 0.4.1 #advanced Simple shell 0.4 +
handle arguments for the built-in exit Usage: exit status, where status is an integer used to exit the shell

setenv, unsetenv #advanced Simple shell 1.0 +
Implement the setenv and unsetenv builtin commands
setenv Initialize a new environment variable, or modify an existing one Command syntax: setenv VARIABLE VALUE Should print something on stderr on failure unsetenv Remove an environment variable Command syntax: unsetenv VARIABLE Should print something on stderr on failure

cd #advanced Simple shell 1.0 +
Implement the builtin command cd:

Changes the current directory of the process. Command syntax: cd [DIRECTORY] If no argument is given to cd the command must be interpreted like cd $HOME You have to handle the command cd - You have to update the environment variable PWD when you change directory man chdir, man getcwd

; #advanced Simple shell 1.0 +
Handle the commands separator ;

&& and || #advanced Simple shell 1.0 +
Handle the && and || shell logical operators

alias #advanced Simple shell 1.0 + Implement the alias builtin command Usage: alias [name[='value'] ...] alias: Prints a list of all aliases, one per line, in the form name='value' alias name [name2 ...]: Prints the aliases name, name2, etc 1 per line, in the form name='value' alias name='value' [...]: Defines an alias for each name whose value is given. If name is already an alias, replaces its value with value

Variables #advanced Simple shell 1.0 +

Handle variables replacement Handle the 
$ variable

Comments #advanced Simple shell 1.0 +
Handle comments (#)

File as input #advanced Simple shell 1.0 +
