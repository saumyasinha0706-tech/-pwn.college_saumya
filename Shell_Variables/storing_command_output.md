# Challenge Name
Storing command output

## My solve
**Flag:** `pwn.college{Yj2cX0PDkUdtfA1hR2V4358wXfe.QX1cDN1wCOwEzNzEzW}`
i used command substitution to run the /challenge/run command and capture its output.then  i stored that output into a variable named pwn. then i got the flag.

```bash

hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{Yj2cX0PDkUdtfA1hR2V4358wXfe.QX1cDN1wCOwEzNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned command substitution.

## References 
None
