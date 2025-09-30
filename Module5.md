# File globbing
## Matching with *
The challenge teaches me about * glob.
**Flag** `pwn.college{cIA8sxDaqsllJgAxwCkyvz_ME_D.QXxIDO0wCMyEzNzEzW}`
```
When it encounters a * character in any argument, the shell will treat it as a "wildcard" and try to replace that argument with any files that match the pattern.
Here,i had to change my directory to /challenge but using  * glob to keep the argument you pass to cd to at most four characters.So, i used cd /ch* command and then invoked /challenge/run to get my flag.
```
### What I learned
I learned to invoke commands and search for files/directories using * glob
### Refernces
The matter in pwn.college


## Matching with ?
The challenge teaches me about * glob.
**Flag** `pwn.college{smHRaqmbX-s_dunCHQ3qA5iIVZ7.QXyIDO0wCMyEzNzEzW}`
```
When it encounters a ? character in any argument, the shell will treat it as a single-character wildcard. This works like *, but only matches one character.
Here,i had to change my directory to /challenge but using ? glob to keep the argument you pass to cd to at most four characters.So, i used cd /?ha??enge command and then invoked /challenge/run to get my flag.
```
### What I learned
I learned to invoke commands and search for files/directories using ? glob
### Refernces
The matter in pwn.college


## Matching with []
The challenge teaches me about [] glob.
**Flag** `pwn.college{E-KVePotIWYWtiPyPczhnFY4h-t.QXzIDO0wCMyEzNzEzW}`
```
The square brackets are, essentially, a limited form of ?, in that instead of matching any character, [] is a wildcard for some subset of potential characters, specified within the brackets.
For example, [pwn] will match the character p, w, or n.
Here,i had to change my directory to /challenge/files run /challenge/run with a single argument that bracket-globs into file_b, file_a, file_s, and file_h. So, i used /challenge/run file_[bash] command to get my flag.
```
### What I learned
I learned to invoke commands and search for files/directories using [] glob
### Refernces
The matter in pwn.college


## Matching paths with []
The challenge teaches me about reaching absolute paths using [] glob.
**Flag** `pwn.college{k_CjpNO17Z8-t9sdoTncd00hE_K.QX0IDO0wCMyEzNzEzW}`
```
Globbing happens on a path basis, so you can expand entire paths with your globbed arguments.
Here,i had to,starting from my home directory, run /challenge/run with a single argument that bracket-globs into the absolute paths to the file_b, file_a, file_s, and file_h files. So, i used  /challenge/run /challenge/files/file_[bash] command to get my flag.
```
### What I learned
I learned to invoke files/directories using absolute paths using [] glob
### Refernces
The matter in pwn.college


## Multiple globs
The challenge teaches me about using multiple globs simultaneausly.
**Flag** `pwn.college{E-PL36s7CoA06LRZAULQIan2fOl.0lM3kjNxwCMyEzNzEzW}`
```
Bash supports the expansion of multiple globs in a single word.
Here,i had to Go cd there and run /challenge/run, providing a single argument: a short (3 characters or less) globbed word with two * globs in it that covers every word that contains the letter p.
So, i used /challenge/run *p* command to get my flag.
```
### What I learned
I learned to invoke files/directories/commands using multiple globs at once.
### Refernces
The matter in pwn.college


## Mixing globs
The challenge teaches me about using mixing globs.
**Flag** `pwn.college{ItuEVuVdC7ss2pwQgDN6CxwlgdX.QX1IDO0wCMyEzNzEzW}`
```
Bash supports the expansion of multiple globs in a single word.
Here,i had to Go Go cd there and, using globbing, write a single, short (6 characters or less) glob that (when passed as an argument to /challenge/run) will match the files "challenging", "educational", and "pwning"!
So, i used  /challenge/run [epc]* command to get my flag.
```
### What I learned
I learned to invoke files/directories/commands using multiple globs at once.
### Refernces
The matter in pwn.college

