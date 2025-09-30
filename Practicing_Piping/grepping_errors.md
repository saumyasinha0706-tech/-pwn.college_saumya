# Challenge Name
Grepping errors

## My solve
**Flag:** `pwn.college{Y4UCzj7Um-Kx9COohL6D2CJhP8B.QX1ATO0wCOwEzNzEzW}`
i used >& to redirect standard error to standard output. i then used the pipe operator and used grep to find the flag.

```bash
 /challenge/run 2>&1 | grep pwn
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwned
pwning
pwns
pwn
pwn.college{Y4UCzj7Um-Kx9COohL6D2CJhP8B.QX1ATO0wCOwEzNzEzW}
```
## Incorrect tangents I went on
NI had trouble understanding how to implement the challenge at first.

## What I learned
I learned about the >& operator, and this challenge was also like a revision of previous challenges.

## References 
None
