# Perceiving permissions
## Changing file ownership
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
