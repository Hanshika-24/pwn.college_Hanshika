# Comprehending commands
## cat command
The challenge teaches me about cat command.
**Flag** `pwn.college{oMdoUSyxr3AJ75Hwf6ZanFZGnxy.QXxcTN0wCMyEzNzEzW}`
``` bash
One of the most critical Linux commands is cat. cat is most often used for reading out files.
cat will concatenate (hence the name) multiple files if provided multiple arguments.
Here,i read the flag file in my home directory using cat.
```
### What I learned
I learned about the the cat command.
### References
The video in pwn.college


## catting absolute paths
The challenge teaches me about specifying cat arguments as absolute paths.
**Flag** `pwn.college{kYH6amULLkcksMXkSyUIWcHVSek.QX5ETO0wCMyEzNzEzW}`
``` bash
We can specify cat arguments as absolute paths.
Here,i read the flag file with cat at its absolute path: /flag.
```
### What I learned
I learned about the the cat command containing absolute paths as argument.
### References
The video in pwn.college


## more catting practice
The challenge gives me more catting practice
**Flag** `pwn.college{4F1LvN86ikGSiY22zDfyNJ9iseX.QXwITO0wCMyEzNzEzW}`
``` bash
We can specify all sorts of paths as arguments to commands.
Here,i could not use cd to open the flag file directory and read flag file but the challenge did not allow using cd. So, i had to provide the absolute path of the flag file as an arguement to the cat command and get the flag.
```
### What I learned
I learned about the the cat command containing absolute paths as argument.
### References
The video in pwn.college


## grepping for a needle in a haystack
The challenge teaches me about grep command
**Flag** `pwn.college{c5rugUMFfFiJh801wof4OqDQG3P.QX3EDO0wCMyEzNzEzW}`
``` bash
We use grep command to search for the contents we need when the files that we might cat out are too big.
Here, i had to search for  the flag out of hundred thousand lines of text in the flag file using grep command to get the flag. I did this using the keyword "pwn.college" which is always t present at the start of all the flags.
```
### What I learned
I learned about the the grep command.
### References
The video in pwn.college


## comparing files
The challenge teaches me about finding difference between 2 files
**Flag** `pwn.college{4CI-n_Zj6611OcUPhMg-9fNvL0X.01MwMDOxwCMyEzNzEzW}`
``` bash
When looking for changes between similar files, eyeballing them might not be the most efficient approach! This is where the diff command becomes invaluable.
diff compares two files line by line and shows you exactly what's different between them.
Here, i used diff to find what's different between the two given files and got my flag.
```
### What I learned
I learned about the the diff command.
### References
The video in pwn.college


## listing files
The challenge teaches me ls command
**Flag** `pwn.college{IEpwj109qHkgBt74ECCZcHGK3oz.QX4IDO0wCMyEzNzEzW}`
``` bash
Directories can have lots of files (and other directories) inside them,and we can use ls command to list the content inside them.
Here, i used diff to find what's different between the two given files and got my flag.
```
### What I learned
I learned how to list all the files in a given directory.
### References
The video in pwn.college


## touching files
The challenge teaches me touch command
**Flag** `pwn.college{gVVKCGU0DwhiU8yGIRQ9acJo6NM.QXwMDO0wCMyEzNzEzW}`
``` bash
We can create a new, blank file by touching it with the touch command.
Here, i used touch command to create to files: /tmp/pwn and /tmp/college, and run /challenge/run to get my flag.
```
### What I learned
I learned how to create files using touch command
### References
The video in pwn.college


## deleting files
The challenge teaches me rm command
**Flag** `pwn.college{07fzXhwzgaSrdLZk2lAJhsGHhKB.QX2kDM1wCMyEzNzEzW}`
``` bash
We can remove a file by deleting it with the rm command.
Here, i used rm command to delete a file: delete_me which i first created to get my flag.
```
### What I learned
I learned how to remove files using rm command
### References
The video in pwn.college


## moving files
The challenge teaches me mv command
**Flag** `pwn.college{cq35dzw2LcqU1DQ7JDkBut5_j0C.0VOxEzNxwCMyEzNzEzW}`
``` bash
We can move around a file  with the mv command.
Here, i used mv command to move the /flag file into /tmp/hack-the-planet to get my flag.
```
### What I learned
I learned how to move files using mv command
### References
The video in pwn.college


## hidden files
The challenge teaches me to view some hidden files
**Flag** `pwn.college{4blJVRNzClDpnF7g1e-jmUCeIWz.QXwUDO0wCMyEzNzEzW}`
``` bash
ls doesn't list all the files by default. Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts. To view them with ls, we need to invoke ls with the -a flag
Here, i used ls -a command to view the flag file which was hidden to get my flag.
```
### What I learned
I learned how view the files beginning with '.' using ls -a command
### References
The video in pwn.college



## An epic filesyste quest
The challenge helps me revise the concept taught till now
**Flag** `pwn.college{kddv7zg_9Lyi5nto5FAK_45qk2j.QX5IDO0wCMyEzNzEzW}`
``` bash
Here, the flag file was hidden and i had to follow a set of clues to get my flag.
```
### What I learned
I brushed up my concepts about ls cat touch commands.
### References
The video in pwn.college


## Making Directories
The challenge teaches me to use mkdir command
**Flag** `pwn.college{oWxjO8g9iRAGlgRk2AZtN_LVtTh.QXxMDO0wCMyEzNzEzW}`
``` bash
We can make directories using the mkdir command. Then we can stick files in there.
Here, i created a /tmp/pwn directory and made  a college file in it to get my flag.
```
### What I learned
I learned how to create directories using mkdir command.
### References
The video in pwn.college


## Finding files
The challenge teaches me to use find command
**Flag** `pwn.college{oWxjO8g9iRAGlgRk2AZtN_LVtTh.QXxMDO0wCMyEzNzEzW}`
``` bash
The find command takes optional arguments describing the search criteria and the search location.
Here, i had to find the flag file on the filesystem which took various attempts of using the find command in different directories get my flag.
```
### What I learned
I learned how to find files using find command.
### References
The video in pwn.college


## Linking files
The challenge teaches me about symbolic links.
**Flag** `pwn.college{4blJVRNzClDpnF7g1e-jmUCeIWz.QXwUDO0wCMyEzNzEzW}`
``` bash
In a filesystem, a file is, conceptually, an address at which the contents of that file live.
A hard link is an alternate address that indexes that data, accesses to the hard link and accesses to the original file are completely identical, in that they immediately yield the necessary data. A soft/symbolic link, instead, contains the original file name.
When you access the symbolic link, Linux will realize that it is a symbolic link, read the original file name, and then (typically) automatically access that file. In most cases, both situations result in accessing the original data, but the mechanisms are different.
Symbolic links are created with the ln command with the -s argument, like so:
Here, i had to find the flag file using symlinks because /challenge/catflag read out /home/hacker/not-the-flag to get my flag.
```
### What I learned
I learned how to use symlinks created using ln command with -s argument.
### References
The video in pwn.college



