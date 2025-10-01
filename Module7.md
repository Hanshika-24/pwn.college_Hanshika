# Shell variables
## Printing varaibles
The challenge teaches me printing variables out.
**Flag** `pwn.college{cIA8sxDaqsllJgAxwCkyvz_ME_D.QXxIDO0wCMyEzNzEzW}`
```bash
We can also print out variables with echo, by prepending the variable name with a $.
For example, there is a variable, PWD, that always holds the current working directory of the current shell.
Here,i had to get my shell print out the FLAG variable to get my flag.
```
### What I learned
I learned to print variables.
### Refernces
The matter in pwn.college



## Setting varaibles
The challenge teaches me how to write values to variables.
**Flag** `pwn.college{cxn2b7oNSWjwRxmANH6HLdwVykk.QX5UTN0wCMyEzNzEzW}`
```bash
Naturally, as well as reading values stored in variables, we can write values to variables.
This is done, as with many other languages, using =. 
Here,i had to  set the PWN variable to the value COLLEGE to get my flag.
```
### What I learned
I learned to assign values to variables.
### Refernces
The matter in pwn.college


## Multi-word varaibles
The challenge teaches me about qouting.
**Flag** `pwn.college{AhZwFVruSVHy8SspVvrzA_zRC7V.QXwYTN0wCMyEzNzEzW}`
```bash
Spaces have special significance in the shell, and there are places where you can't use them spuriously.
When the shell sees a space, it ends the variable assignment and interprets the next word (SAUCE in this case) as a command. To set them as a variable, we need to qoute it.
Here,i had to  set the variable PWN to COLLEGE YEAH to get my flag.
```
### What I learned
I learned to assign multi-word values to variables.
### Refernces
The matter in pwn.college


## Exporting varaibles
The challenge teaches me about exporting.
**Flag** `pwn.college{Ig1jxxAJmlb01QdIZZbEPs_j4Ut.QXyYTN0wCMyEzNzEzW}`
```bash
When we export variables, they are passed into the environment variables of child processes. We'll encounter the concept of environment variables in other challenges, but we'll observe their effects here.
Here,i had to  invoke /challenge/run with the PWN variable exported and set to the value COLLEGE, and the COLLEGE variable set to the value PWN but not exported to get my flag.
```
### What I learned
I learned to export variables.
### Refernces
The matter in pwn.college


## Printing exported varaibles
The challenge teaches me about printing exported variables.
**Flag** `pwn.college{0I34YnCnHrppI3bn41ojGW0CVzJ.QX4UTN0wCMyEzNzEzW}`
```bash
There are multiple ways to access variables in bash. 
Here,i had to  use env command which printed out every exported variable set and i had to search to get my flag.
```
### What I learned
I learned to print exported variables.
### Refernces
The matter in pwn.college


## Storing command output
The challenge teaches me about storing outputs.
**Flag** `pwn.college{QhRU9BcZaPjsiuJlLV4cR4lGUw3.QX1cDN1wCMyEzNzEzW}`
```bash
The shell makes storing outputs quite easy using something called Command Substitution
Here,i had to Read the output of the /challenge/run command directly into a variable called PWN to get my flag.
```
### What I learned
I learned to print store outputs of commands.
### Refernces
The matter in pwn.college


## Reading input
The challenge teaches me about reading inputs.
**Flag** `pwn.college{UgCUZ6EkI6WWutwvnlmUTk1phbX.QX4cTN0wCMyEzNzEzW}`
```bash
Reading input from the user is done using the aptly named read builtin, which reads input into a variable.
read reads data from your standard input.
Here,i had to use read to set the PWN variable to the value COLLEGE to get my flag.
```
### What I learned
I learned to print read inputs using read.
### Refernces
The matter in pwn.college


## Reading files
The challenge teaches me how to read files.
**Flag** `pwn.college{cIA8sxDaqsllJgAxwCkyvz_ME_D.QXxIDO0wCMyEzNzEzW}`
```bash
Running a whole other program just to read the file is a waste. It turns out that we can just use the powers of the shell.
Here,i had to read /challenge/read_me into the PWN environment variable to get my flag.
```
### What I learned
I learned to print read files using read and redirection.
### Refernces
The matter in pwn.college


