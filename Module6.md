# Practicing Piping
## Redirecting output
The challenge teaches me how to redirect output.
**Flag** `pwn.college{Ux_at8kkTJtYhdbhzmN7FMcvz0R.QX0YTN0wCMyEzNzEzW}`
```bash
We can redirect stdout to files with the > character.
Here,i had to do output redirection to write the word PWN (all uppercase) to the filename COLLEGE (all uppercase).So, i used echo PWN > COLLEGE to get my flag.
```
### What I learned
I learned to redirect outputs using > character.
### References
The matter in pwn.college



## Redirecting more output
The challenge teaches me how to redirect output at a deeper level.
**Flag** `pwn.college{ATIlTYU9hGprzKjHrNOoRpIFege.QX1YTN0wCMyEzNzEzW}`
```
Aside from redirecting the output of echo,we can also redirect the output of any command.
Here,i had to do output redirection from /challenge/rum file to myflag file.So, i used /challenge/run > myflag comand then cat myflag to get my flag.
```
### What I learned
I learned to redirect outputs of commands.
### References
The matter in pwn.college



## Appending output
The challenge teaches me how to append outputs.
**Flag** `pwn.college{guELmYCeAKgz87mSmIkEad4p0gS.QX3ATO0wCMyEzNzEzW}`
```bash
A common use-case of output redirection is to save off some command results for later analysis.
Often times, we want to do this in aggregate: run a bunch of commands, save their output, and grep through it later. In this case, we might want all that output to keep appending to the same file, but > will create a new output file every time, deleting the old contents.
We can redirect input in append mode using >> instead of >.
Here,i had to append output to get my flag. So, i used /challenge/run >> /home/hacker/the-flag comand to append.
```
### What I learned
I learned to appending outputs using >> character.
### References
The matter in pwn.college


## Redirecting errors
The challenge teaches me how to redirect errors.
**Flag** `pwn.college{wdkCO-vzJ-EQIr5mAfnphiTtahg.QX3YTN0wCMyEzNzEzW}`
```bash
Just like standard output, you can also redirect the error channel of commands.
A File Descriptor (FD) is a number that describes a communication channel in Linux.
Here,i had to redirect the output of /challenge/run to myflag, and the instructions to instructions. So, i used /challenge/run 1>myflag 2>instructions command and then cat instructions and cat myflag to get the flag.
```
### What I learned
I learned to redirect errors using > character.
### References
The matter in pwn.college



## Redirecting input
The challenge teaches me how to redirect input.
**Flag** `pwn.college{k6O8gEcJ92wC3Phh4PAbEBXD0gW.QXwcTN0wCMyEzNzEzW}`
```bash
Just like redirecting outputs,we can also redirect inputs to programs using < character.
Here,i had to first use echo COLLEGE > PWN command to have the PWN file contain the value COLLEGE and then /challenge/run < PWN command to redirect the PWN file to /challenge/run to get the flag.
```
### What I learned
I learned to redirect inputs using < character.
### References
The matter in pwn.college


## Grepping stored results
The challenge teaches me how to search between results.
**Flag** `pwn.college{QcUNV3i147jwBqzMGa2G_TeIAMT.QX4EDO0wCMyEzNzEzW}`
```bash
Here,i had to redirect the output of /challenge/run to /tmp/data.txt which resulted in a hundred thousand lines of text, with one of them being the flag, in /tmp/data.txt and then grep for the flag. So, i used /challenge/run > /tmp/data.txt command first then grep pwn /tmp/data.txt to search for the flag and then get the flag.
```
### What I learned
I learned to perform multiple operations of redirections including grepping.
### References
The matter in pwn.college


## Grepping live output
The challenge teaches me how to search between results.
**Flag** `pwn.college{kNrlbHEL-JhGl4Ash9SYjy3shHZ.QX5EDO0wCMyEzNzEzW}`
```bash
To cut out the middleman we can use the pipe operator.
Standard output from the command to the left of the pipe will be connected to (piped into) the standard input of the command to the right of the pipe. 
Here, /challenge/run  output a hundred thousand lines of text, including the flag.So, i used /challenge/run | grep pwn.college command  to grep and get the flag.
```
### What I learned
I learned to grep outputs.
### References
The matter in pwn.college



## Grepping errors
The challenge teaches me how to grep errors.
**Flag** `pwn.college{kNrlbHEL-JhGl4Ash9SYjy3shHZ.QX5EDO0wCMyEzNzEzW}`
```bash
The > operator redirects a given file descriptor to a file.
The shell has a >& operator, which redirects a file descriptor to another file descriptor. This means that we can have a two-step process to grep through errors: first, we redirect standard error to standard output (2>& 1) and then pipe the now-combined stderr and stdout as normal (|)
Here, get the output to grep through to get the flag.
```
### What I learned
I learned to grep errors.
### References
The matter in pwn.college

## Filtering with grep -v
The challenge teaches me how to filter with grep -v.
**Flag** `pwn.college{kNrlbHEL-JhGl4Ash9SYjy3shHZ.QX5EDO0wCMyEzNzEzW}`
```bash
The grep command has a very useful option: -v (invert match). While normal grep shows lines that MATCH a pattern, grep -v shows lines that do NOT match a pattern.
Here,i had to grep -v to filter out all the lines containing "DECOY" to get the flag.
```
### What I learned
I learned to filter using grep -v.
### References
The matter in pwn.college


## Duplicating piper data with tee
The challenge teaches me how to duplicate data.
**Flag** `pwn.college{kNrlbHEL-JhGl4Ash9SYjy3shHZ.QX5EDO0wCMyEzNzEzW}`
```bash
The tee command, named after a "T-splitter" from plumbing pipes, duplicates data flowing through your pipes to any number of files provided on the command line.
Here,i had to grep -v to filter out all the lines containing "DECOY" to get the flag.
```
### What I learned
I learned to use tee to duplicate data.
### References
The matter in pwn.college


## Process substitution for input
The challenge teaches me compare the output of two commands rather than two files.
**Flag** `pwn.college{kNrlbHEL-JhGl4Ash9SYjy3shHZ.QX5EDO0wCMyEzNzEzW}`
```bash
We can hook input and output of programs to arguments of commands. This is done using Process Substitution.
For reading from a command (input process substitution), use <(command). 
Here,i had to process substitution with diff to compare the outputs of these two programs to get the flag.
```
### What I learned
I learned to do pro ess substitution.
### References
The matter in pwn.college


## Writing to multiple programs
The challenge teaches me process substitution for writing to commands.
**Flag** `pwn.college{kNrlbHEL-JhGl4Ash9SYjy3shHZ.QX5EDO0wCMyEzNzEzW}`
```bash
If we write an argument of >(rev), bash will run the rev command (this command reads data from standard input, reverses its order, and writes it to standard output!), but hook up its input to a temporary named pipe file.
When commands write to this file, the data goes to the standard input of the command
Here,i had to Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands to get the flag.
```
### What I learned
I learned to use process substitution for writing to commands.
### References
The matter in pwn.college



## Split-piping stderr and stdout
The challenge teaches me process substitution for writing to commands.
**Flag** `pwn.college{kNrlbHEL-JhGl4Ash9SYjy3shHZ.QX5EDO0wCMyEzNzEzW}`
```bash
If we write an argument of >(rev), bash will run the rev command (this command reads data from standard input, reverses its order, and writes it to standard output!), but hook up its input to a temporary named pipe file.
When commands write to this file, the data goes to the standard input of the command
Here,i had to Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands to get the flag.
```
### What I learned
I learned to use process substitution for writing to commands.
### References
The matter in pwn.college



## Named pipes
The challenge teaches me process substitution for writing to commands.
**Flag** `pwn.college{kNrlbHEL-JhGl4Ash9SYjy3shHZ.QX5EDO0wCMyEzNzEzW}`
```bash
If we write an argument of >(rev), bash will run the rev command (this command reads data from standard input, reverses its order, and writes it to standard output!), but hook up its input to a temporary named pipe file.
When commands write to this file, the data goes to the standard input of the command
Here,i had to Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands to get the flag.
```
### What I learned
I learned to use process substitution for writing to commands.
### References
The matter in pwn.college


