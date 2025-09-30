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
