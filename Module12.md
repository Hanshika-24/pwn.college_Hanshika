# Chaining commands
## Chaining with semicolons
The challenge teaches me how to chain commands.
### My solve
**Flag** `pwn.college{IS8cW3jaYn7uBuy3ZluYKqTfVew.QX1UDO0wCMyEzNzEzW}`
```bash
The easiest way to chain commands is ;. In most contexts, ; separates commands in a similar way to how Enter separates lines.
Here,i had to use the /challenge/pwn; /challenge/college to get the flag.
```
### What I learned
I learned about chaining commands using semicolons.
### References
The matter in pwn.college


## Building on Success
The challenge teaches me how to chain commands.
### My solve
**Flag** `pwn.college{spM4GSMhpslv4CQg625BzBcX2yn.0lM0MDOxwCMyEzNzEzW}`
```bash
The && operator allows you to run a second command only if the first command succeeds (in Linux convention, this means it exited with code 0). This is called the "AND" operator because both conditions must be true: the first command must succeed AND then the second command will run. That's super useful for complex commandline workflows where certain actions depend on the success of other actions.
Here,i had to use the /challenge/first-success && /challenge/second command to get the flag.
```
### What I learned
I learned about chaining commands using and operator.
### References
The matter in pwn.college


## Handling failure
The challenge teaches me how to chain commands.
### My solve
**Flag** `pwn.college{svER9X_-Kp6Nigj5F-wChpwpiWa.01M0MDOxwCMyEzNzEzW}`
```bash
The || operator allows you to run a second command only if the first command fails (exits with a non-zero code). This is called the "OR" operator because either the first command succeeds OR the second command will run.
Here,i had to use the /challenge/first-failure || /challenge/second command to get the flag.
```
### What I learned
I learned about chaining commands using or operator.
### References
The matter in pwn.college


## Your first shell script
The challenge teaches me how to create shell scripts.
### My solve
**Flag** `pwn.college{kp9lsmL8rAtKJjFoeyb9mYjwE9x.QXxcDO0wCMyEzNzEzW}`
```bash
We can create a shell script called pwn.sh (by convention, shell scripts are frequently named with a sh suffix).
And then we can execute by passing it as an argument to a new instance of our shell (bash)! When a shell is invoked like this, rather than taking commands from the user, it reads commands from the file.
Here, i first created a script x.sh usinn nano x.sh then executed it using bash x.sh to get the flag.
```
### What I learned
I learned to create shell scripts.
### References
The matter in pwn.college


## Redirecting script output
The challenge teaches me how to redirect script output.
### My solve
**Flag** `pwn.college{kZDWQTbNAis0d8AbZL69e5v5uCq.QX4ETO0wCMyEzNzEzW}`
```bash
As far as the shell is concerned, our script is just another command.
That means we can redirect its input and output just like we did for commands in the Piping module.
Here, i used bash x.sh | /challenge/solve command to  pipe the output of the script into a single invocation of the /challenge/solve command to get the flag.
```
### What I learned
I learned about piping script outputs.
### References
The matter in pwn.college


## Executable shell scripts
The challenge teaches me how to execute shell scripts.
### My solve
**Flag** `pwn.college{o39OgDEPgN5jimz-IoI4AmuDy7z.QX0cjM1wCMyEzNzEzW}`
```bash
We can can simply invoke it via its relative or absolute path.
And then we can execute by passing it as an argument to a new instance of our shell (bash)! When a shell is invoked like this, rather than taking commands from the user, it reads commands from the file.
Here, i first created a scripy y.sh containing /challenge/college and using nano y.sh and then i did ./y.sh to get my flag.
```
### What I learned
I learned how to invoke scripts without bash using absolute paths.
### References
The matter in pwn.college


## Understanding shebangs
The challenge teaches me abput shebangs.
### My solve
**Flag** `pwn.college{kHNd_PHWlX1pGQi8S8F7wiO5-1w.0VOzMDOxwCMyEzNzEzW}`
```bash
When a program is invoked in Linux, the Linux kernel first inspects the file to determine how it should be run. This does NOT use the extension.
There are a bunch of different types of programs, but if the program file starts with the characters #! (often termed a "shebang"), Linux treats the file as an interpreted program, and the contents of the rest of the line as the path to the interpreter. It then invokes the interpreter with the path to the program file as its only argument.
Here, i first used nano solve.sh command to create a script containing #!/bin/bash and echo "hack the planet" then made it executable with chmod a+x solve.sh command then did /challenge/run to get the flag.
```
### What I learned
I learned about using shebangs to define file types.
### References
The matter in pwn.college


## Scripting with arguments
The challenge teaches me how to provide arguments to scripts.
### My solve
**Flag** `pwn.college{cBd-LdNdbVPQTvTB1kFR2qMrx5_.0VNzMDOxwCMyEzNzEzW}`
```bash
Scripts become much more powerful when they can accept arguments.
Here i first created a script using nano solve.sh command containing
 [ #!/bin/bash
echo "$2 $1" ].
Then i used bash solve.sh pwn college comand to check the output which ws correctly "college pwn". So i used /challenge/run command to get the flag.
```
### What I learned
I learned about running scripts with arguments.
### References
The matter in pwn.college


## Scripting with conditionals
The challenge teaches me how to provide conditions to scripts.
### My solve
**Flag** `pwn.college{MqzrsPsB-anI9x8OnT75laI3rC1.0lNzMDOxwCMyEzNzEzW}`
```bash
We can use if statements to make decisions.
Here i first created a script using nano solve.sh command containing
 [ #!/bin/bash
if [ "$1" == "pwn" ]
then
    echo "college"
fi ].
Then i used bash solve.sh pwn comand to check the output which ws correctly "college". So i used /challenge/run command to get the flag.
```
### What I learned
I learned about running scripts with conditions.
### References
The matter in pwn.college


## Scripting with Default cases
The challenge teaches me how to provide conditions to scripts.
### My solve
**Flag** `pwn.college{URP8x9KyNJDP2QUx6emfju08Qo4.01NzMDOxwCMyEzNzEzW}`
```bash
if statements so far have handled specific cases, but to handle everything else else comes in.
The else clause executes when the if condition is false.
Here i first created a script using nano solve.sh command containing
 [ #!/bin/bash
if [ "$1" == "pwn" ]
then
    echo "college"
else
    echo "nope"
fi ].
Then i used bash solve.sh pwn comand to check the output which ws correctly "college". So i used /challenge/run command to get the flag.
```
### What I learned
I learned about running scripts with conditions including default cases.
### References
The matter in pwn.college



## Scripting with Multiple conditions
The challenge teaches me how to provide multiple conditions to scripts.
### My solve
**Flag** `pwn.college{svER9X_-Kp6Nigj5F-wChpwpiWa.01M0MDOxwCMyEzNzEzW}`
```bash
Here i first created a script using nano solve.sh command containing
 [ #!/bin/bash
if [ "$1" == "pwn" ]
then
    echo "college"
elif [ "$1" == "hack" ]
then
    echo "planet"
if [ "$1" == "learn" ]
then
    echo "linux"
else
    echo "unknown"
fi ].
Then i used bash solve.sh pwn comand to check the output which was correctly "college" and so on. So i used /challenge/run command to get the flag.
```
### What I learned
I learned about running scripts with conditions using if, elif and else.
### References
The matter in pwn.college


## Reading shell scripts
The challenge teaches me how to chain commands.
### My solve
**Flag** `pwn.college{svER9X_-Kp6Nigj5F-wChpwpiWa.01M0MDOxwCMyEzNzEzW}`
```bash
Reading shell scripts are very handy for doing simple "system-level" tasks, and are a common tool that developers and sysadmins reach for. In fact, a surprising fraction of the programs on a typical Linux machine are shell scripts.


```
### What I learned
I learned about chaning commands using semicolons.
### References
The matter in pwn.college
