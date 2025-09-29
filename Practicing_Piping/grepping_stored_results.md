# Challenge Name
Grepping stored results

## My solve
**Flag:** `pwn.college{MXeOBfH827HRXBtfCsOfVUve5ha.QX4EDO0wCOwEzNzEzW}`
I redirected the output as said in the challenge and in order to find the flag i used grep pwn because thats what the flag starts with.

```bash
 /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep pwn /tmp/data.txt
pwning
pwn.college{MXeOBfH827HRXBtfCsOfVUve5ha.QX4EDO0wCOwEzNzEzW}
pwn
pwns
pwned

```
## Incorrect tangents I went on
None

## What I learned
I learned about grepping stored results

## References 
None
