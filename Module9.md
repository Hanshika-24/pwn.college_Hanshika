# Proesses and Jobs
## Listing Processes
The challenge teaches me to list running processes.
### My solve
**Flag** `pwn.college{QB1Vq_pYmQNQrpKvggNwvxn-oEg.QX4MDO0wCMyEzNzEzW}`
```bash
ps either stands for "process snapshot" or "process status", and it lists processes.
By default, ps just lists the processes running in the terminal
Here, i used ps -ef command to find the exact name of flag directory and then run it to get the flag.
```
### What I learned
I learned to use ps command to list running processes.
### References
The matter in pwn.college


## Killing Processes
The challenge teaches me to terminate processes.
### My solve
**Flag** `pwn.college{odWdALcUttT6Q0hmNzB9dAHSV6K.QXyQDO0wCMyEzNzEzW}`
```bash
Processes are terminated using the aggressively-named kill command.
With default options kill will terminate a process in a way that gives it a chance to get its affairs in order before ceasing to exist.
Here, i used ps -ef | grep /challenge/dont_run command find the dont_run process and kill 136 command to kill it.Then /challenge/run command to get the flag.
```
### What I learned
I learned to use ps command to terminate running processes.
### References
The matter in pwn.college


## Interrupting Processes
The challenge teaches me to get rid of processes.
### My solve
**Flag** `pwn.college{QD-Pejl5kGZtGdcuub9VqR6_TMo.QXzQDO0wCMyEzNzEzW}`
```bash
Terminals have a hotkey for this: Ctrl-C (e.g., holding down the Ctrl key and pressing C) sends an "interrupt" to whatever application is waiting on input from the terminal and, typically, this causes the application to cleanly exit.
Here,  /challenge/run did not give the flag until i interrupted it with Ctrl-C to get the flag.
```
### What I learned
I learned to use keys to interrupt running processes.
### References
The matter in pwn.college



## Killing misbehaving Processes
The challenge teaches me to get rid of processes.
### My solve
**Flag** `pwn.college{UPfZemkZp25_Zjt0WeqGzqiNNxt.0FNzMDOxwCMyEzNzEzW}`
```bash
Here,  ps -ef to the get the PID of challenge/decoy and then killed it to get the flag.
```
### What I learned
I learned to use keys to interrupt running processes.
### References
The matter in pwn.college


## Suspending Processes
The challenge teaches me to get rid of processes.
### My solve
**Flag** `pwn.college{wY4wcrfi691SQEwRxL9LwLrnswQ.QX1QDO0wCMyEzNzEzW}`
```bash
Instead of interrupting processes with Ctrl-C,we can suspend processes to the background with Ctrl-Z.
Here, /challenge/run wanted an another copy of itself running and using the same terminal,so i used Ctrl-z key to get the flag.
```
### What I learned
I learned to use keys to suspend running processes.
### References
The matter in pwn.college



## Resuming Processes
The challenge teaches me to resume suspended processes.
### My solve
**Flag** `pwn.college{gVQH3uSLlH3B8h1qdAgqTsxf0ZN.QX2QDO0wCMyEzNzEzW}`
```bash
The fg command is a builtin that takes the suspended process, resumes it, and puts it back in the foreground of the terminal.
Here, /challenge/run wanted to be suspended, then resumed,so i used Ctrl-z key and then fg command to get the flag.
```
### What I learned
I learned to use keys to  resume suspended running processes in foreground.
### References
The matter in pwn.college


## Backgrounding Processes
The challenge teaches me to resume suspended processes in the background.
### My solve
**Flag** `pwn.college{Ybu0ZbaIY7jAyctgYkIGHzwtL-m.QX3QDO0wCMyEzNzEzW}`
```bash
We can resume processes in the background with the bg command.
It will allow the process to keep running, while giving the shell back to invoke more commands in the meantime.
Here, /challenge/run wanted to be suspended, then resumed in background, so i used Ctrl-z key and then bg command to get the flag.
```
### What I learned
I learned to use keys to  resume suspended running processes in background.
### References
The matter in pwn.college


## Foregrounding Processes
The challenge teaches me to resume suspended processes in the background.
### My solve
**Flag** `pwn.college{okW81ubDjyGiWbxU0PgQbELA_BR.QX4QDO0wCMyEzNzEzW}`
```bash
We can resume processes in the background with the bg command.
It will allow the process to keep running, while giving the shell back to invoke more commands in the meantime.
Here, /challenge/run wanted to be suspended, then resumed in foreground, so i used Ctrl-z key and then bg command and subsequently fg command to get the flag.
```
### What I learned
I learned to use keys to  resume suspended running processes in background.
### References
The matter in pwn.college



## Starting Backgrounded Processes
The challenge teaches me to resume suspended processes in the background.
### My solve
**Flag** `pwn.college{oXRsCvnfBCpH1Zw1VMwlYs2hJ7-.QX5QDO0wCMyEzNzEzW}}`
```bash
We can resume processes in the background with the bg command.
It will allow the process to keep running, while giving the shell back to invoke more commands in the meantime.
Here, /challenge/run wanted to be suspended, then resumed in foreground, so i used Ctrl-z key and then bg command and subsequently fg command to get the flag.
```
### What I learned
I learned to use keys to  resume suspended running processes in background.
### References
The matter in pwn.college



## Process Exit Codes
The challenge teaches me to resume suspended processes in the background.
### My solve
**Flag** `pwn.college{oXRsCvnfBCpH1Zw1VMwlYs2hJ7-.QX5QDO0wCMyEzNzEzW}}`
```bash
We can resume processes in the background with the bg command.
It will allow the process to keep running, while giving the shell back to invoke more commands in the meantime.
Here, /challenge/run wanted to be suspended, then resumed in foreground, so i used Ctrl-z key and then bg command and subsequently fg command to get the flag.
```
### What I learned
I learned to use keys to  resume suspended running processes in background.
### References
The matter in pwn.college




