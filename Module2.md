# Pondering paths
## The root
The challenge asks me to invoke the pwn program using its absolute path.
### My solve
**Flag** `pwn.college{chxWA-giWP16WQ6NXKYbX4Uj2E7.QX4cTO0wCMyEzNzEzW}`
```
The filesystem starts at /. Under that, there are a whole mess of other directories, configuration files, programs, and, most importantly, flags.
We can invoke a program by providing its path on the command line.
Here,i refered to the root directory and pwn directory inside it using its absolute path and got a flag.
```
### What I learned
I learned about the linux filesystem and it's root.
### References
The video in pwn.college


## Program and absolute paths
The challenge asks me to invoke the run program using its absolute path.
### My solve
**Flag** `pwn.college{EjlF0QJ9aKAu9CcM8Oau0Vhfe_N.QX1QTN0wCMyEzNzEzW}`
```
We can refer to files and directories by their path which is of two types: absolute and relative.
Here,i refered to the root directory then challenge directory inside and then the run program inside it using its absolute path and got a flag.
```
### What I learned
I learned to invoke files and programs using their paths.
### References
The video in pwn.college


## Position thy self
The challenge asks me to invoke the run program in a specific directory.
### My solve
**Flag** `pwn.college{0nBLicQ0XktvXrIouMB78sY5STF.QX2QTN0wCMyEzNzEzW}`
```bash
The Linux filesystem has tons of directories with tons of files. We can navigate around directories by using the cd (change directory) command and passing a path to it as an argument.
Each process has a directory in which it's currently hanging out and we must ensure the correct  "current working directory" of the process.
Here,i invoked the /challenge/run program from the /proc/132$ directory which i had to find out to get a flag.
```
### What I learned
I learned to cd to the specific program(opening it) before running the challenge.
### References
The video in pwn.college


## Position elsewhere
The challenge asks me to invoke the run program in an unknown directory.
### My solve
**Flag** `pwn.college{MQ7LMW-KOg2TiLMXC7V7fhM4U4L.QX3QTN0wCMyEzNzEzW}`
```bash
Here,i invoked the /challenge/run program from the / (root) directory which i had to find out to get a flag.
```
### What I learned
I learned to cd to the specific program(opening it) before running the challenge.
### References
The video in pwn.college

## Position yet elsewhere
The challenge asks me to invoke the run program in an unknown directory.
### My solve
**Flag** `pwn.college{URHlpitE2FUzh0mIv0hNZQDXnQS.QX4QTN0wCMyEzNzEzW}`
```bash
Here,i invoked the /challenge/run program from the /var/log directory which i had to find out to get a flag.
```
### What I learned
I learned to cd to the specific program(opening it) before running the challenge.
### References
The video in pwn.college

## Implicit relative paths, from /
The challenge asks me to invoke the run program in an unknown directory using relative path.
### My solve
**Flag** `pwn.college{wzs0A0726Q6qILWRVsdmLbSZYfx.QX5QTN0wCMyEzNzEzW}`
```bash
If we put in absolute paths everywhere, then it really doesn't matter what directory we are in. But, the current working directory does matter for relative paths.
A relative path is any path that does not start at root (i.e., it does not start with /).
Here,i invoked the challenge/run program from the / directory using its relative path which i had to find out to get a flag.
```
### What I learned
I learned implicit relative paths.
### References
The video in pwn.college


## Explicit relative paths, from /
The challenge asks me to invoke the run program in an unknown directory using explicit relative path.
### My solve
**Flag** `pwn.college{8CR8VpU3WHj8inIupv6E6D2txxs.QXwUTN0wCMyEzNzEzW}`
```bash
In linux,every directory has two implicit entries that you can refer in paths: . and .. 
Here,i invoked the ./challenge/run program from the / directory using its relative path which i had to find out to get a flag.
```
### What I learned
I learned explicit relative paths.
### References
The video in pwn.college


## Implicit relative paths
The challenge asks me to invoke the run program in an unknown directory using implicit relative path.
### My solve
**Flag** `pwn.college{woGxzdlW8m7C50b1-F7fQo5Ifw8.QXxUTN0wCMyEzNzEzW}`
```bash
Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path because if linux searched the current directory for programs everytime you entered a naked path, it could accidentally execute programs in your current directory that happened to have the same names as core system utilities!
Here,i invoked the ./run program from the /challenge directory using its relative path which i had to find out to get a flag.

```
### What I learned
I learned implicit relative paths.
### References
The video in pwn.college


## Home sweet home
The challenge asks me to invoke the  /challenge/run as it  writes a copy of the flag to any file i specify as an argument on the commandline, with some constraints.
### My solve
**Flag** `pwn.college{k_BDxkMYcp7inpChy1H2XHg-klC.QXzMDO0wCMyEzNzEzW}`
```bash
Every user has a home directory, typically under /home in the filesystem.
The home directory is typically where users store most of their personal files.
~ is the shorthand for /home/hacker.Thus, whenever bash sees ~ provided as the start of an argument in a way consistent with a path, it will expand it to your home directory.
Here,i invoked the executed the /challenge/run program with `/f as an argument so that it write a copy of the flag in this file whose absolute path i provided to get a flag.
```
### What I learned
I learned the basics of linux file  paths.
### References
The video in pwn.college
