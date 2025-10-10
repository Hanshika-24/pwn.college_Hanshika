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
**Flag** `pwn.college{o9NPqJSNXbV1Y2DpzqauReazoqu.QXzcjM1wCMyEzNzEzW}`
```bash
Like ownership, file permissions can also be changed. This is done with the chmod (change mode) command. 
Here,i ls -l /flag to check the current permissions of flag file then i used chmod o+r /flag command to get access to it and thencat /flag  to get the flag.
```
### What I learned
I learned about chmod command.
### References
The video in pwn.college


## Executible files
The challenge teaches me how to change user access to files.
### My solve
**Flag** `pwn.college{c0dVnYCT2ArsnGcvWedsKG8TNhU.QXyEjN0wCMyEzNzEzW}`
```bash
Here,i used ls -l /challenge/run to check the current permissions of flag file then i used chmod a+x /challenge/run command to get access to it and then /challenge/run  to get the flag.
```
### What I learned
I learned about chmod command.
### References
The video in pwn.college


## Permission tweaking practice
The challenge teaches me how to change permissions.
### My solve
**Flag** `pwn.college{0IcB5s3aKZJ7Xf5gtLRaEi1LDvG.QXwEjN0wCMyEzNzEzW}`
```bash
Here,i used the following commmands get the flag according to instructions displayed:
chmod go+w /challenge/pwn
chmod ug+x /challenge/pwn
chmod o-w /challenge/pwn
chmod g-wx /challenge/pwn
chmod u-rwx /challenge/pwn
chmod a-rwx /challenge/pwn
chmod u=x,g=x,o= /challenge/pwn	
chmod u=rx,g=x,o=rx /challenge/pwn
chmod u+r /flag
cat /flag
```
### What I learned
I learned about chmod command.
### References
The video in pwn.college



## Permission Setting practice
The challenge teaches me how to set permissions.
### My solve
**Flag** `pwn.college{ks71Gn2p9hHmrfVQlTV_zVYx9BE.QXzETO0wCMyEzNzEzW}`
```bash
chmod can also simply set permissions altogether, overwriting the old ones. This is done by using = instead of - or +.
Here,i used the following commmands get the flag according to instructions displayed:
chmod u=r,g=rwx,o=w /challenge/pwn
chmod u=w,g=w,o=x /challenge/pwn
chmod u=rw,g=rx,o=rw /challenge/pwn
chmod u=r,g=rw,o=wx /challenge/pwn
chmod u=rwx,g=x,o=rwx /challenge/pwn
chmod u=x,g=r,o=rwx /challenge/pwn
chmod u=x,g=w,o=x /challenge/pwn
chmod u=w,g=x,o= /challenge/pwn
chmod u+r /flag
cat /flag

```
### What I learned
I learned about chmod command.
### References
The video in pwn.college


## The SUID bit
The challenge teaches me about SUID bits.
### My solve
**Flag** `pwn.college{c0dVnYCT2ArsnGcvWedsKG8TNhU.QXyEjN0wCMyEzNzEzW}`
```bash
The system admin can't be there to give them the password every time a user wanted to do a task that only root/sudoers can do. Instead, the "Set User ID" (SUID) permissions bit allows the user to run a program as the owner of that program's file.
Here, i used chmod u+s /challenge/getrot command to add SUID BIT and then /challenge/getroot to spawn a root shell and then cat /flag to get the flag.
```
### What I learned
I learned about chmod command.
### References
The video in pwn.college




