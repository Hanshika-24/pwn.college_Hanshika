# Data Manipulation
## Translating characters
The challenge teaches me how to modify data.
### My solve
**Flag** `pwn.college{EOzi3RKqqkj279LXu1JC3RiTPZ3.01MxEzNxwCMyEzNzEzW}`
```bash
tr translates characters it receives over standard input and prints them to standard output.
In its most basic usage, tr translates the character provided in its first argument to the character provided in its second argument
It can also handle multiple characters, with the characters in different positions of the first argument replaced with associated characters in the second argument.
Here, /challenge/run printed the flag after swaping the casing of all characters,so i had to undo it with tr to get the flag.
So, i first used /challenge/run command which gave me the swapped flag as output then i used echo PWN.COLLEGE{eoZI3rkQQKJ279lxU1jc3rItpz3.01mXeZnXWcmYeZnZeZw} | tr ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ
which gave the correct flag as output.
```
### What I learned
I learned to use tr command to modify data.
### References
The matter in pwn.college


## Deleting characters
The challenge teaches me how to modify data.
### My solve
**Flag** `pwn.college{cXddebIXTIefo04h-3HcBHVOOou.0FNxEzNxwCMyEzNzEzW}`
```bash
tr can also translate characters to nothing (i.e., delete them). This is done via a -d flag and an argument of what characters to delete.
So, i first used /challenge/run command which gave me the  flag with extra ^% as output then i used echo p^%w^n^.%c%o^l%l^%e^%ge{^%c^X%d^d^%e^%b^IX^T%I^%e%f^%o^%0^%4^%h^-^3^H^%c^%B^%HV%O^Oo^u^.^%0%F^%Nx%E^%z%N^xw%C^%M%y%E^%z%N%z%E^%z%W%}^^ | tr -d ^% command which gave me the correct flag as output.
```
### What I learned
I learned to use tr -d command to modify data.
### References
The matter in pwn.college


## Deleting newlines
The challenge teaches me how to modify data.
### My solve
**Flag** `pwn.college{wMUE_VCL8dnWXVFeBeSV1CpV4Sw.0VNxEzNxwCMyEzNzEzW}`
```bash
A common class of characters to remove is a line separator.
We can specify newlines almost like any other character, by escaping them.
Here, i first used /challenge/run command which gave me the  flag with new lines as output then i used e echo "p
w
n.
co
ll
eg
e{
w
M
U
E
_V
C
L
8d
n
WXV
F
e
Be
S
V
1
W}" | tr -d "\n"
 command which gave me the correct flag as output.
```
### What I learned
I learned to use tr -d "\n" command to delete lines from data.
### References
The matter in pwn.college


## Extracting the first lines with head.
The challenge teaches me how to extract from data.
### My solve
**Flag** `pwn.college{oOSn4u6oA8EpAfAp7buiCvl3NSW.0lNxEzNxwCMyEzNzEzW}`
```bash
The head command is used to display the first few lines of its input.
So, i used /challenge/pwn | head -n 7 | /challenge/college command to filter only first 7 lines from /challenge/pwn and then | character to pipe it to /challenge/college to get the flag.
```
### What I learned
I learned to use head command to extract few lines from data.
### References
The matter in pwn.college


## Extracting specific sections of text
The challenge teaches me how to extract from data.
### My solve
**Flag** `pwn.college{ghvOK1aAINUj0t-J4y6PHQCt1jm.01NxEzNxwCMyEzNzEzW}`
```bash
cut command is used to grab specific columns of data.
The -d argument specifies the column delimiter (how columns are separated).
So, i used /challenge/run | cut -d " " -f 2 | tr -d "\n" command to extract the 2nd column from /challenge/run and tr to remove next line character to get the flag.
```
### What I learned
I learned to use head command to extract few columns from data and modify it.
### References
The matter in pwn.college


## Sorting data
The challenge teaches me how to sort data.
### My solve
**Flag** `pwn.college{gj-ABl6ksReJaGeCT2EiqciSXlr.0FM0MDOxwCMyEzNzEzW}`
```bash
The sort command helps to organize data. It reads lines from input (or files) and outputs them in sorted order.
So, i used sort /challenge/flags.txt command to sort the file alphabetically to get the flag.
```
### What I learned
I learned to use sort command.
### References
The matter in pwn.college
