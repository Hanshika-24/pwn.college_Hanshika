# Terminal Multiplexing
## Launching screen
The challenge teaches me how to start screens.
### My solve
**Flag** `pwn.college{ATyrACl_Fq5nMXpN0SuQykXn3C6.0VN4IDOxwCMyEzNzEzW}`
```bash
screen is a program that creates virtual terminals inside the terminal.
It's somewhat like having multiple browser tabs, but for your command line
Here, i had to use screen command to start a screen and then exit it to get my flag.
```
### What I learned
I learned about screens.
### References
The matter in pwn.college


## Detaching and attaching
The challenge teaches me how to start screens.
### My solve
**Flag** `pwn.college{ATyrACl_Fq5nMXpN0SuQykXn3C6.0VN4IDOxwCMyEzNzEzW}`
```bash
We detach by pressing Ctrl-A, followed by d (for detach). This leaves the session running in the background while we return to our normal terminal.
To reattach, we can use the -r argument to screen.
Here, i had to use screen command to start a screen and then deattach it and then run /challenge/run and then reattach  to get my flag.
```
### What I learned
I learned about deattaching and reattaching from screens.
### References
The matter in pwn.college


## Finding sessions
The challenge teaches me how to find particular screens.
### My solve
**Flag** `pwn.college{wq9cQiHKF-KOZbeAHuOzcFtpQ7v.01N4IDOxwCMyEzNzEzW}`
```bash
We detach by pressing Ctrl-A, followed by d (for detach). This leaves the session running in the background while we return to our normal terminal.
To reattach, we can use the -r argument to screen.
Here, i had to use screen -ls command to see a list of screen and their ids then nagivate through them by attaching and detaching to get my flag.
```
### What I learned
I learned about searching particular screens.
### References 
The matter in pwn.college


## Switching windows
The challenge teaches me how to find particular screens.
### My solve
**Flag** `pwn.college{kAmUpn6DaGhbn7VCULOlmKekGx1.0FO4IDOxwCMyEzNzEzW}`
```bash
Inside a single screen session, we can have multiple windows, like a browser has multiple tabs. This can be super handy for organizing different tasks.
Here, i had to use screen -r command to reattach to the  screen and then navigate to window 0 of it using ctr-a 0 button  to get my flag.
```
### What I learned
I learned about switchig between terminals within screens.
### References 
The matter in pwn.college


## Detaching and attaching(tmux)
The challenge teaches me how to use tmux to Deattach and attach.
### My solve
**Flag** `pwn.college{0n2kfuPdCW4T5NlWsI_nYGv4x-b.0VO4IDOxwCMyEzNzEzW}`
```bash
tmux (terminal multiplexer) is screen's younger, more modern cousin. It does all the same things but with some different key bindings.
Instead of Ctrl-A, tmux uses Ctrl-B as its command prefix.
Here, i had to use tmux command to start a tmux and then deattach it and then run /challenge/run and then reattach  to get my flag.
```
### What I learned
I learned about starting tmux.
### References 
The matter in pwn.college


## Switching windows(tmux)
The challenge teaches me how to Switch windows in tmux.
### My solve
**Flag** `pwn.college{8Rwxty7c504LfaI5OHZ97uXhFke.0FM5IDOxwCMyEzNzEzW}`
```bash
Tmux shows your windows at the bottom in a status bar.
Here, i had to use tmux a command to reattach to the tmux and then navigate to window 0 of it using ctr-b 0 button  to get my flag.
```
### What I learned
I learned about navigating windows in tmux.
### References 
The matter in pwn.college
