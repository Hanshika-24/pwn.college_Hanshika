# Pondering path
## The PATH variable
The challenge teaches me about PATH variable.
### My solve
**Flag** `pwn.college{ATyrACl_Fq5nMXpN0SuQykXn3C6.0VN4IDOxwCMyEzNzEzW}`
```bash
There is a special shell variable, called PATH, that stores a bunch of directory paths in which the shell will search for programs corresponding to commands.
If we blank out the variable, things go badly.
Here, i had to use PATH="" command to make sure rm command does not find the path to /flag and then i used /challenge/run get my flag.
```
### What I learned
I learned about PATH.
### References
The matter in pwn.college


## Setting PATH
The challenge teaches me about uses of PATH variable.
### My solve
**Flag** `pwn.college{kDtsn-Tu6FSfVTvv8LTIr2rTlGb.QX1cjM1wCMyEzNzEzW}`
```bash
By adding directories to or replacing directories in this list, you can expose these programs to be launched using their bare name.
Here, i had to use PATH=/challenge/more_commands/ command to make sure win is in PATH  then i used /challenge/run win get my flag.
```
### What I learned
I learned about using PATH for our benefits.
### References
The matter in pwn.college


## Finding commands
The challenge teaches me to find commands executed particularly.
### My solve
**Flag** `pwn.college{gaQv2U5fi0rTi2aNfUG0GpGll-b.01NzEzNxwCMyEzNzEzW}`
```bash
Mirroring what the shell does when searching for commands, which looks at each directory in $PATH in order and prints the first file it finds whose name matches the argument passed.
Here, i had to use which win command to find out which directory flag is in. Then i used cat /challenge/paths/28323/flag to get my flag.
```
### What I learned
I learned about which command.
### References
The matter in pwn.college


## Adding commands
The challenge teaches me to add commands.
### My solve
**Flag** `pwn.college{gaQv2U5fi0rTi2aNfUG0GpGll-b.01NzEzNxwCMyEzNzEzW}`
```bash
Mirroring what the shell does when searching for commands, which looks at each directory in $PATH in order and prints the first file it finds whose name matches the argument passed.

```
### What I learned
I learned about which command.
### References
The matter in pwn.college


## Hijacking commands
The challenge teaches me to edit commands.
### My solve
**Flag** `pwn.college{gaQv2U5fi0rTi2aNfUG0GpGll-b.01NzEzNxwCMyEzNzEzW}`
```bash

```
### What I learned
I learned about which command.
### References
The matter in pwn.college


