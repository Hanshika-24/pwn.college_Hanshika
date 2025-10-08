# Untangling Users
## Becoming root with su
The challenge teaches me how to become the root user.
### My solve
**Flag** `pwn.college{w1n5Hx-wv0eh6CVG8pAxpAMvtvW.QX2UDN1wCMyEzNzEzW}`
```bash
It's not just hackers that need to become root. Oftentimes the owner of your computer, need to use root access to administer it. Becoming root is a fairly common action that Linux users take, and there are two utilities that exist for this purpose: su and sudo.
su (the substitute user command) is not typically used to elevate to root access anymore, but it is an elegant utility from a more civilized time.
Here,i first used the root password to get root user access using su command then used ls command to find the directory containing flag and used cat myflag to get the flag.
```
### What I learned
I learned about su command which is used to become the root user.
### References
The video in pwn.college


## Other users with su
The challenge teaches me how to become the other user using su.
### My solve
**Flag** `pwn.college{w1n5Hx-wv0eh6CVG8pAxpAMvtvW.QX2UDN1wCMyEzNzEzW}`
```bash
With no arguments, su will start a root shell (after authenticating with root's password). However, we can also give a username as an argument to switch to that user instead of root. 
Here,i first used  su zardus command and put in the password to become zardus user then did /challenge/run to get the flag.
```
### What I learned
I learned about su command which can also be used to become any user.
### References
The video in pwn.college



## Cracking passwords
The challenge teaches me how to find secret passwords.
### My solve
**Flag** `pwn.college{EpUuTh2hVKMBYm2a-lJdUeIiL2R.QX3UDN1wCMyEzNzEzW}`
```bash
Passwords used to be stored in /etc/passwd, but because /etc/passwd is a globally-readable file, this is not good for passwords, these were moved to /etc/shadow.
Separated by :s, the first field of each line is the username and the second is the password. A value of * or ! functionally means that password login for the account is disabled, a blank field means that there is no password (a not-uncommon misconfiguration that allows password-less su in some configurations), and the long string is the result of one-way-encrypting (hashing) Zardus' password from the last level. 
Here,i  first found zarus' hash using cat /challenge/shadow-leak command,also used john /challenge/shadow-leak command and then used  su zardus command and put in the password to become zardus user then did /challenge/run to get the flag.
```
### What I learned
I learned about su command which can also be used find secret passwords using hash.
### References
The video in pwn.college


## Using sudo
The challenge teaches me how to find secret passwords.
### My solve
**Flag** `pwn.college{I070dwt2FxDOA8Jk0n7HH7XDWwy.QX4UDN1wCMyEzNzEzW}`
```bash
Root passwords are a pain to maintain, they (or their hashes!) can leak, and they don't lend themselves well to larger environments (e.g., fleets of servers). To address this, in recent decades, the world has moved from administration via su to administration via sudo.
su stands for "substitute user", the current meaning of sudo is "substitute user, do".
Unlike su, which relies on password authentication, sudo checks policies to determine whether the user is authorized to run commands as root. These policies are defined in /etc/sudoers.
Here,i first used  sudo whoami command to check if i have the access as the root user and then sudo cat /flag command get the flag.
```
### What I learned
I learned about sudo command which can also be used to become any user without password.
### References
The video in pwn.college




