# Challenge Name
Grepping live output

## My solve
**Flag:** `pwn.college{Q8WHvD8kwZSIiqkMcUYnfZCehF6.QX5EDO0wCOwEzNzEzW}`
I used the pipe operator as said in the challenge and used grep to find the flag.


```bash
/challenge/run | grep pwn
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwn
pwn.college{Q8WHvD8kwZSIiqkMcUYnfZCehF6.QX5EDO0wCOwEzNzEzW}
pwns
pwning
pwned
```
## Incorrect tangents I went on
i made syntax errors 

## What I learned
I learned about pipe operator 

## References 
None
