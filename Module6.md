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




