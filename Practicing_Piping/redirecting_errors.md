# Challenge Name
Redirecting errors

## My solve
**Flag:** `pwn.college{41sAsXQPGoLIF8UZ_uzAt-QX4uq.QX3YTN0wCOwEzNzEzW}`
According to the challenge ihad to use fd to redirect both standard output and standard error.  I redirected standard output to the myflag file and standard error  to the instructions file using the command /challenge/run > myflag 2> instructions.

```bash
 /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat myflag
cat instructions

[FLAG] Here is your flag:
[FLAG] pwn.college{41sAsXQPGoLIF8UZ_uzAt-QX4uq.QX3YTN0wCOwEzNzEzW}

[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
```
## Incorrect tangents I went on
None

## What I learned
I learned about redirecting errors.

## References 
None
