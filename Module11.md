# Perceiving permissions
## Changing file ownership
The challenge teaches me how to change user acess to files.
### My solve
**Flag** `pwn.college{UzpGy5MDXTY2_9R31OA2S4YaTgi.QXxEjN0wCMyEzNzEzW}`
```bash
We can change the ownership of files via the chown (change owner) command.
Here,i first used  chown hacker /flag command to change owner of /flag file then cat /flag to get the flag.
```
### What I learned
I learned about chown command.
### References
The video in pwn.college


## Groups and files
The challenge teaches me how to change user acess to groups.
### My solve
**Flag** `pwn.college{EW8j93J_HJCqaO0CPnahjjGX6kq.QXxcjM1wCMyEzNzEzW}`
```bash
Sharing is caring, and sharing is built into Linux's design. Files have both an owning user and group. A group can have multiple users in it, and a user can be a member of multiple groups.
We can check what groups you are part of with the id command.
Group ownership can be changed with the chgrp (change group) command.
Here,i first used  chgrp hacker /flag command to change group of /flag file then cat /flag to get the flag.
```
### What I learned
I learned about chgrp command.
### References
The video in pwn.college



## Fun with Group Names
The challenge teaches me how to change groups.
### My solve
**Flag** `pwn.college{MGIvLM7jbkySjKS9tue01S0Maxd.QXycjM1wCMyEzNzEzW}`
```bash
Here,i first used id command to find my group then chgrp grp17401 /flag command to change group of /flag file then cat /flag to get the flag.
```
### What I learned
I learned about id command.
### References
The video in pwn.college


## Changing permissions
The challenge teaches me how to change groups.
### My solve
**Flag** `pwn.college{MGIvLM7jbkySjKS9tue01S0Maxd.QXycjM1wCMyEzNzEzW}`
```bash
Like ownership, file permissions can also be changed. This is done with the chmod (change mode) command. 
Here,i  to get the flag.
```
### What I learned
I learned about id command.
### References
The video in pwn.college
